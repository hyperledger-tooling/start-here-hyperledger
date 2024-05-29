---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/547" class=".btn">#547</a>
            </td>
            <td>
                <b>
                    Bump prettier from 3.0.3 to 3.2.5 in /oid4vci/integration/afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [prettier](https://github.com/prettier/prettier) from 3.0.3 to 3.2.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/releases">prettier's releases</a>.</em></p>
<blockquote>
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
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md">prettier's changelog</a>.</em></p>
<blockquote>
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
const template = &quot;foobar&quot;;
<p><a href="https://github.com/Component"><code>@​Component</code></a>({
[template]: <code>&amp;lt;h1&amp;gt;{{       hello }}&amp;lt;/h1&amp;gt;</code>,
})
export class AppComponent {}
&lt;/tr&gt;&lt;/table&gt;
</code></pre></p>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prettier/prettier/commit/7142cf354cce2558f41574f44b967baf11d5b603"><code>7142cf3</code></a> Release 3.2.5</li>
<li><a href="https://github.com/prettier/prettier/commit/8cbee2e217baad7acf4cb3947834e8c1b41ed647"><code>8cbee2e</code></a> chore(deps): update glimmer to v0.88.1 (<a href="https://redirect.github.com/prettier/prettier/issues/15991">#15991</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/45baee061cb982d9dd298fefa74f4c195a3e0709"><code>45baee0</code></a> chore(deps): update dependency magic-string to v0.30.6 (<a href="https://redirect.github.com/prettier/prettier/issues/16022">#16022</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/9fb32a1a6b10bfb6dae317492f10e5e42956cf23"><code>9fb32a1</code></a> Minor refactor to property print (<a href="https://redirect.github.com/prettier/prettier/issues/15924">#15924</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/08f19401e48ccfeddff4300827da4c8677cb2b79"><code>08f1940</code></a> Update install script for husky v9 (<a href="https://redirect.github.com/prettier/prettier/issues/16000">#16000</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/6d0b1d2a935d47e0517721a0d5e62eb79e972b0c"><code>6d0b1d2</code></a> Update yarn to v4.1.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16021">#16021</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/c8ba8dbca18858a7962184bbb3898502b9ec7cfb"><code>c8ba8db</code></a> chore(deps): update dependency <code>@​angular/compiler</code> to v17.1.2 (<a href="https://redirect.github.com/prettier/prettier/issues/16018">#16018</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/e2250ec6881222a1bb46ef55403067a259d8c7a3"><code>e2250ec</code></a> chore(deps): update typescript-eslint to v6.20.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16015">#16015</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/02865f6cc77858b3a4cbaf7d4e2e72a4e88fe175"><code>02865f6</code></a> chore(deps): update dependency npm-run-all2 to v6.1.2 (<a href="https://redirect.github.com/prettier/prettier/issues/16017">#16017</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/014ee5d47445ae79233291d5b4846b28bedf3601"><code>014ee5d</code></a> chore(deps): update dependency hermes-parser to v0.19.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16014">#16014</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/prettier/prettier/compare/3.0.3...3.2.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=prettier&package-manager=npm_and_yarn&previous-version=3.0.3&new-version=3.2.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:18:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/546" class=".btn">#546</a>
            </td>
            <td>
                <b>
                    Bump pytest-asyncio from 0.23.6 to 0.23.7 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.6 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.6...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.6&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:18:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/545" class=".btn">#545</a>
            </td>
            <td>
                <b>
                    Bump react-dom from 18.2.0 to 18.3.1 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react-dom](https://github.com/facebook/react/tree/HEAD/packages/react-dom) from 18.2.0 to 18.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react/releases">react-dom's releases</a>.</em></p>
<blockquote>
<h2>18.3.1 (April 26, 2024)</h2>
<ul>
<li>Export <code>act</code> from <code>react</code> <a href="https://github.com/facebook/react/commit/f1338f8080abd1386454a10bbf93d67bfe37ce85">f1338f</a></li>
</ul>
<h2>18.3.0 (April 25, 2024)</h2>
<p>This release is identical to 18.2 but adds warnings for deprecated APIs and other changes that are needed for React 19.</p>
<p>Read the <a href="https://react.dev/blog/2024/04/25/react-19-upgrade-guide">React 19 Upgrade Guide</a> for more info.</p>
<h3>React</h3>
<ul>
<li>Allow writing to <code>this.refs</code> to support string ref codemod <a href="https://github.com/facebook/react/commit/9090712fd3ca4e1099e1f92e67933c2cb4f32552">909071</a></li>
<li>Warn for deprecated <code>findDOMNode</code> outside StrictMode <a href="https://github.com/facebook/react/commit/c3b283964108b0e8dbcf1f9eb2e7e67815e39dfb">c3b283</a></li>
<li>Warn for deprecated <code>test-utils</code> methods <a href="https://github.com/facebook/react/commit/d4ea75dc4258095593b6ac764289f42bddeb835c">d4ea75</a></li>
<li>Warn for deprecated Legacy Context outside StrictMode <a href="https://github.com/facebook/react/commit/415ee0e6ea0fe3e288e65868df2e3241143d5f7f">415ee0</a></li>
<li>Warn for deprecated string refs outside StrictMode <a href="https://redirect.github.com/facebook/react/pull/25383">#25383</a></li>
<li>Warn for deprecated <code>defaultProps</code> for function components <a href="https://redirect.github.com/facebook/react/pull/25699">#25699</a></li>
<li>Warn when spreading <code>key</code> <a href="https://redirect.github.com/facebook/react/pull/25697">#25697</a></li>
<li>Warn when using <code>act</code> from <code>test-utils</code> <a href="https://github.com/facebook/react/commit/d4ea75dc4258095593b6ac764289f42bddeb835c">d4ea75</a></li>
</ul>
<h3>React DOM</h3>
<ul>
<li>Warn for deprecated <code>unmountComponentAtNode</code> <a href="https://github.com/facebook/react/commit/8a015b68cc060079878e426610e64e86fb328f8d">8a015b</a></li>
<li>Warn for deprecated <code>renderToStaticNodeStream</code> <a href="https://redirect.github.com/facebook/react/pull/28874">#28874</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react/blob/main/CHANGELOG.md">react-dom's changelog</a>.</em></p>
<blockquote>
<h2>18.3.1 (April 26, 2024)</h2>
<ul>
<li>Export <code>act</code> from <code>react</code> <a href="https://github.com/facebook/react/commit/f1338f8080abd1386454a10bbf93d67bfe37ce85">f1338f</a></li>
</ul>
<h2>18.3.0 (April 25, 2024)</h2>
<p>This release is identical to 18.2 but adds warnings for deprecated APIs and other changes that are needed for React 19.</p>
<p>Read the <a href="https://react.dev/blog/2024/04/25/react-19-upgrade-guide">React 19 Upgrade Guide</a> for more info.</p>
<h3>React</h3>
<ul>
<li>Allow writing to <code>this.refs</code> to support string ref codemod <a href="https://github.com/facebook/react/commit/9090712fd3ca4e1099e1f92e67933c2cb4f32552">909071</a></li>
<li>Warn for deprecated <code>findDOMNode</code> outside StrictMode <a href="https://github.com/facebook/react/commit/c3b283964108b0e8dbcf1f9eb2e7e67815e39dfb">c3b283</a></li>
<li>Warn for deprecated <code>test-utils</code> methods <a href="https://github.com/facebook/react/commit/d4ea75dc4258095593b6ac764289f42bddeb835c">d4ea75</a></li>
<li>Warn for deprecated Legacy Context outside StrictMode <a href="https://github.com/facebook/react/commit/415ee0e6ea0fe3e288e65868df2e3241143d5f7f">415ee0</a></li>
<li>Warn for deprecated string refs outside StrictMode <a href="https://redirect.github.com/facebook/react/pull/25383">#25383</a></li>
<li>Warn for deprecated <code>defaultProps</code> for function components <a href="https://redirect.github.com/facebook/react/pull/25699">#25699</a></li>
<li>Warn when spreading <code>key</code> <a href="https://redirect.github.com/facebook/react/pull/25697">#25697</a></li>
<li>Warn when using <code>act</code> from <code>test-utils</code> <a href="https://github.com/facebook/react/commit/d4ea75dc4258095593b6ac764289f42bddeb835c">d4ea75</a></li>
</ul>
<h3>React DOM</h3>
<ul>
<li>Warn for deprecated <code>unmountComponentAtNode</code> <a href="https://github.com/facebook/react/commit/8a015b68cc060079878e426610e64e86fb328f8d">8a015b</a></li>
<li>Warn for deprecated <code>renderToStaticNodeStream</code> <a href="https://redirect.github.com/facebook/react/pull/28874">#28874</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/react/commit/d6c42f7b1134c4f033296ce4d47a7803aa0929df"><code>d6c42f7</code></a> Bump to 18.3.1</li>
<li><a href="https://github.com/facebook/react/commit/8a015b68cc060079878e426610e64e86fb328f8d"><code>8a015b6</code></a> Add deprecation warning for unmountComponentAtNode</li>
<li><a href="https://github.com/facebook/react/commit/c3b283964108b0e8dbcf1f9eb2e7e67815e39dfb"><code>c3b2839</code></a> Add deprecation warning for findDOMNode</li>
<li><a href="https://github.com/facebook/react/commit/d4ea75dc4258095593b6ac764289f42bddeb835c"><code>d4ea75d</code></a> ReactDOMTestUtils deprecation warnings</li>
<li><a href="https://github.com/facebook/react/commit/7548c019ce44e41301555aac645fbdfcf180e9b9"><code>7548c01</code></a> Deprecate <code>renderToStaticNodeStream</code> (<a href="https://github.com/facebook/react/tree/HEAD/packages/react-dom/issues/28872">#28872</a>) (<a href="https://github.com/facebook/react/tree/HEAD/packages/react-dom/issues/28874">#28874</a>)</li>
<li><a href="https://github.com/facebook/react/commit/589423270e8d69fce914f12f7dc7bb61bb7b81de"><code>5894232</code></a> Enable warning for defaultProps on function components for everyone (<a href="https://github.com/facebook/react/tree/HEAD/packages/react-dom/issues/25699">#25699</a>)</li>
<li><a href="https://github.com/facebook/react/commit/c2a246e956a164c7a92a3807c973bf9b56f85a6b"><code>c2a246e</code></a> Turn on string ref deprecation warning for everybody (not codemoddable) (<a href="https://github.com/facebook/react/tree/HEAD/packages/react-dom/issues/25383">#25383</a>)</li>
<li><a href="https://github.com/facebook/react/commit/2cfb4741fdf2f9e3a843930d95ee6965fab44b8f"><code>2cfb474</code></a> Bump version from 18.2 to 18.3</li>
<li>See full diff in <a href="https://github.com/facebook/react/commits/v18.3.1/packages/react-dom">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~react-bot">react-bot</a>, a new releaser for react-dom since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-dom&package-manager=npm_and_yarn&previous-version=18.2.0&new-version=18.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:18:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/544" class=".btn">#544</a>
            </td>
            <td>
                <b>
                    Bump requests from 2.32.1 to 2.32.2 in /kafka_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.32.1 to 2.32.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.2</h2>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li>See full diff in <a href="https://github.com/psf/requests/compare/v2.32.1...v2.32.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.32.1&new-version=2.32.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:18:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/543" class=".btn">#543</a>
            </td>
            <td>
                <b>
                    Bump pytest-asyncio from 0.23.6 to 0.23.7 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.6 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.6...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.6&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/542" class=".btn">#542</a>
            </td>
            <td>
                <b>
                    Bump pytest-asyncio from 0.23.6 to 0.23.7 in /connection_update/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.6 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.6...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.6&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/541" class=".btn">#541</a>
            </td>
            <td>
                <b>
                    Bump react from 18.2.0 to 18.3.1 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react](https://github.com/facebook/react/tree/HEAD/packages/react) from 18.2.0 to 18.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react/releases">react's releases</a>.</em></p>
<blockquote>
<h2>18.3.1 (April 26, 2024)</h2>
<ul>
<li>Export <code>act</code> from <code>react</code> <a href="https://github.com/facebook/react/commit/f1338f8080abd1386454a10bbf93d67bfe37ce85">f1338f</a></li>
</ul>
<h2>18.3.0 (April 25, 2024)</h2>
<p>This release is identical to 18.2 but adds warnings for deprecated APIs and other changes that are needed for React 19.</p>
<p>Read the <a href="https://react.dev/blog/2024/04/25/react-19-upgrade-guide">React 19 Upgrade Guide</a> for more info.</p>
<h3>React</h3>
<ul>
<li>Allow writing to <code>this.refs</code> to support string ref codemod <a href="https://github.com/facebook/react/commit/9090712fd3ca4e1099e1f92e67933c2cb4f32552">909071</a></li>
<li>Warn for deprecated <code>findDOMNode</code> outside StrictMode <a href="https://github.com/facebook/react/commit/c3b283964108b0e8dbcf1f9eb2e7e67815e39dfb">c3b283</a></li>
<li>Warn for deprecated <code>test-utils</code> methods <a href="https://github.com/facebook/react/commit/d4ea75dc4258095593b6ac764289f42bddeb835c">d4ea75</a></li>
<li>Warn for deprecated Legacy Context outside StrictMode <a href="https://github.com/facebook/react/commit/415ee0e6ea0fe3e288e65868df2e3241143d5f7f">415ee0</a></li>
<li>Warn for deprecated string refs outside StrictMode <a href="https://redirect.github.com/facebook/react/pull/25383">#25383</a></li>
<li>Warn for deprecated <code>defaultProps</code> for function components <a href="https://redirect.github.com/facebook/react/pull/25699">#25699</a></li>
<li>Warn when spreading <code>key</code> <a href="https://redirect.github.com/facebook/react/pull/25697">#25697</a></li>
<li>Warn when using <code>act</code> from <code>test-utils</code> <a href="https://github.com/facebook/react/commit/d4ea75dc4258095593b6ac764289f42bddeb835c">d4ea75</a></li>
</ul>
<h3>React DOM</h3>
<ul>
<li>Warn for deprecated <code>unmountComponentAtNode</code> <a href="https://github.com/facebook/react/commit/8a015b68cc060079878e426610e64e86fb328f8d">8a015b</a></li>
<li>Warn for deprecated <code>renderToStaticNodeStream</code> <a href="https://redirect.github.com/facebook/react/pull/28874">#28874</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react/blob/main/CHANGELOG.md">react's changelog</a>.</em></p>
<blockquote>
<h2>18.3.1 (April 26, 2024)</h2>
<ul>
<li>Export <code>act</code> from <code>react</code> <a href="https://github.com/facebook/react/commit/f1338f8080abd1386454a10bbf93d67bfe37ce85">f1338f</a></li>
</ul>
<h2>18.3.0 (April 25, 2024)</h2>
<p>This release is identical to 18.2 but adds warnings for deprecated APIs and other changes that are needed for React 19.</p>
<p>Read the <a href="https://react.dev/blog/2024/04/25/react-19-upgrade-guide">React 19 Upgrade Guide</a> for more info.</p>
<h3>React</h3>
<ul>
<li>Allow writing to <code>this.refs</code> to support string ref codemod <a href="https://github.com/facebook/react/commit/9090712fd3ca4e1099e1f92e67933c2cb4f32552">909071</a></li>
<li>Warn for deprecated <code>findDOMNode</code> outside StrictMode <a href="https://github.com/facebook/react/commit/c3b283964108b0e8dbcf1f9eb2e7e67815e39dfb">c3b283</a></li>
<li>Warn for deprecated <code>test-utils</code> methods <a href="https://github.com/facebook/react/commit/d4ea75dc4258095593b6ac764289f42bddeb835c">d4ea75</a></li>
<li>Warn for deprecated Legacy Context outside StrictMode <a href="https://github.com/facebook/react/commit/415ee0e6ea0fe3e288e65868df2e3241143d5f7f">415ee0</a></li>
<li>Warn for deprecated string refs outside StrictMode <a href="https://redirect.github.com/facebook/react/pull/25383">#25383</a></li>
<li>Warn for deprecated <code>defaultProps</code> for function components <a href="https://redirect.github.com/facebook/react/pull/25699">#25699</a></li>
<li>Warn when spreading <code>key</code> <a href="https://redirect.github.com/facebook/react/pull/25697">#25697</a></li>
<li>Warn when using <code>act</code> from <code>test-utils</code> <a href="https://github.com/facebook/react/commit/d4ea75dc4258095593b6ac764289f42bddeb835c">d4ea75</a></li>
</ul>
<h3>React DOM</h3>
<ul>
<li>Warn for deprecated <code>unmountComponentAtNode</code> <a href="https://github.com/facebook/react/commit/8a015b68cc060079878e426610e64e86fb328f8d">8a015b</a></li>
<li>Warn for deprecated <code>renderToStaticNodeStream</code> <a href="https://redirect.github.com/facebook/react/pull/28874">#28874</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/react/commit/f1338f8080abd1386454a10bbf93d67bfe37ce85"><code>f1338f8</code></a> Export <code>React.act</code> from 18.3</li>
<li><a href="https://github.com/facebook/react/commit/d6c42f7b1134c4f033296ce4d47a7803aa0929df"><code>d6c42f7</code></a> Bump to 18.3.1</li>
<li><a href="https://github.com/facebook/react/commit/73bfaa16e1487d6c4a83ca960a6f0365af2ab440"><code>73bfaa1</code></a> Turn on key spread warning in jsx-runtime for everyone (<a href="https://github.com/facebook/react/tree/HEAD/packages/react/issues/25697">#25697</a>)</li>
<li><a href="https://github.com/facebook/react/commit/c2a246e956a164c7a92a3807c973bf9b56f85a6b"><code>c2a246e</code></a> Turn on string ref deprecation warning for everybody (not codemoddable) (<a href="https://github.com/facebook/react/tree/HEAD/packages/react/issues/25383">#25383</a>)</li>
<li><a href="https://github.com/facebook/react/commit/2cfb4741fdf2f9e3a843930d95ee6965fab44b8f"><code>2cfb474</code></a> Bump version from 18.2 to 18.3</li>
<li>See full diff in <a href="https://github.com/facebook/react/commits/v18.3.1/packages/react">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~react-bot">react-bot</a>, a new releaser for react since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react&package-manager=npm_and_yarn&previous-version=18.2.0&new-version=18.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/540" class=".btn">#540</a>
            </td>
            <td>
                <b>
                    Bump pytest-asyncio from 0.23.6 to 0.23.7 in /kafka_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.6 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.6...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.6&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/539" class=".btn">#539</a>
            </td>
            <td>
                <b>
                    Bump typescript from 5.2.2 to 5.4.5 in /oid4vci/integration/afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [typescript](https://github.com/Microsoft/TypeScript) from 5.2.2 to 5.4.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/Microsoft/TypeScript/releases">typescript's releases</a>.</em></p>
<blockquote>
<h2>TypeScript 5.4.5</h2>
<p>For release notes, check out the <a href="https://devblogs.microsoft.com/typescript/announcing-typescript-5-4/">release announcement</a>.</p>
<p>For the complete list of fixed issues, check out the</p>
<ul>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.0%22+is%3Aclosed+">fixed issues query for Typescript 5.4.0 (Beta)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.1%22+is%3Aclosed+">fixed issues query for Typescript 5.4.1 (RC)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.2%22+is%3Aclosed+">fixed issues query for Typescript 5.4.2 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.3%22+is%3Aclosed+">fixed issues query for Typescript 5.4.3 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.4%22+is%3Aclosed+">fixed issues query for Typescript 5.4.4 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.5%22+is%3Aclosed+">fixed issues query for Typescript 5.4.5 (Stable)</a>.</li>
</ul>
<p>Downloads are available on:</p>
<ul>
<li><a href="https://www.nuget.org/packages/Microsoft.TypeScript.MSBuild">NuGet package</a></li>
</ul>
<h2>TypeScript 5.4.4</h2>
<p>For release notes, check out the <a href="https://devblogs.microsoft.com/typescript/announcing-typescript-5-4/">release announcement</a>.</p>
<p>For the complete list of fixed issues, check out the</p>
<ul>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.0%22+is%3Aclosed+">fixed issues query for Typescript 5.4.0 (Beta)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.1%22+is%3Aclosed+">fixed issues query for Typescript 5.4.1 (RC)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.2%22+is%3Aclosed+">fixed issues query for Typescript 5.4.2 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.3%22+is%3Aclosed+">fixed issues query for Typescript 5.4.3 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.4%22+is%3Aclosed+">fixed issues query for Typescript 5.4.4 (Stable)</a>.</li>
</ul>
<p>Downloads are available on:</p>
<ul>
<li><a href="https://www.nuget.org/packages/Microsoft.TypeScript.MSBuild">NuGet package</a></li>
</ul>
<h2>TypeScript 5.4.3</h2>
<p>For release notes, check out the <a href="https://devblogs.microsoft.com/typescript/announcing-typescript-5-4/">release announcement</a>.</p>
<p>For the complete list of fixed issues, check out the</p>
<ul>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.0%22+is%3Aclosed+">fixed issues query for Typescript 5.4.0 (Beta)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.1%22+is%3Aclosed+">fixed issues query for Typescript 5.4.1 (RC)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.2%22+is%3Aclosed+">fixed issues query for Typescript 5.4.2 (Stable)</a>.</li>
<li><a href="https://github.com/Microsoft/TypeScript/issues?utf8=%E2%9C%93&amp;q=milestone%3A%22TypeScript+5.4.3%22+is%3Aclosed+">fixed issues query for Typescript 5.4.3 (Stable)</a>.</li>
</ul>
<p>Downloads are available on:</p>
<ul>
<li><a href="https://www.nuget.org/packages/Microsoft.TypeScript.MSBuild">NuGet package</a></li>
</ul>
<h2>TypeScript 5.4</h2>
<p>For release notes, check out the <a href="https://devblogs.microsoft.com/typescript/announcing-typescript-5-4/">release announcement</a>.</p>
<p>For the complete list of fixed issues, check out the</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/microsoft/TypeScript/commit/27bcd4cb5a98bce46c9cdd749752703ead021a4b"><code>27bcd4c</code></a> Update LKG</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/9f33bf1cd586a4028928d30b1bfe521788ec4da4"><code>9f33bf1</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58098">#58098</a> (Fix constraints of nested homomorph...) into release-5.4 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/71b2f84741f94e1414e41af8c65293a030d39945"><code>71b2f84</code></a> Bump version to 5.4.5 and LKG</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/892936f4a18ded0216ae1c805a9890ebb8572fe3"><code>892936f</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/58083">#58083</a> (Don't propagate partial union/inter...) into release-5.4 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/38a7c0587df926957d3a6e808c62c6332665572d"><code>38a7c05</code></a> release-5.4: Always set node-version for setup-node (<a href="https://redirect.github.com/Microsoft/TypeScript/issues/58117">#58117</a>)</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/b754fc393738ae05aad136324a0dc78787745644"><code>b754fc3</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/57778">#57778</a> (fix type import check for default-i...) into release-5.4 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/8eb3367164dd9cdc9c0b85424ed39ab28eff2312"><code>8eb3367</code></a> Bump version to 5.4.4 and LKG</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/de9096b42b052ffabbf2b46b573557e7c2eb259d"><code>de9096b</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/57871">#57871</a> (Divide-and-conquer strategy for int...) into release-5.4 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/06aae9839d7160c2aff8c3f14b9f1f2d3e76c2d4"><code>06aae98</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/57973">#57973</a> (Compare package.json paths with cor...) into release-5.4 (#...</li>
<li><a href="https://github.com/microsoft/TypeScript/commit/6d8134e5afe0661ff97f2ad1f0e0341087d58908"><code>6d8134e</code></a> 🤖 Pick PR <a href="https://redirect.github.com/Microsoft/TypeScript/issues/57637">#57637</a> (Fixed a regression related to deter...) into release-5.4 (#...</li>
<li>Additional commits viewable in <a href="https://github.com/Microsoft/TypeScript/compare/v5.2.2...v5.4.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=typescript&package-manager=npm_and_yarn&previous-version=5.2.2&new-version=5.4.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/538" class=".btn">#538</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.1 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/66ff8dffdf9eee9b3dd6686de34542c49ff80dcd"><code>66ff8df</code></a> Prepare release version 8.2.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3ffcfd122cf4674ac45f6233d9b50be6c49abeea"><code>3ffcfd1</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12340">#12340</a> from pytest-dev/backport-12334-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0b28313b46a04de08bddc18896b3e61312a0c5b3"><code>0b28313</code></a> [8.2.x] Add Python 3.13 (beta) support</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f3dd93ad8d62eb0a260d3090f31be82aafbcff13"><code>f3dd93a</code></a> [8.2.x] Attest package provenance (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12335">#12335</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bb5a1257b0aafe5932377fa8e9fd92ab39418ac7"><code>bb5a125</code></a> [8.2.x] Spelling (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12331">#12331</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f179bf252fe2c1d0afce64b4b4bab4449e366e84"><code>f179bf2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12327">#12327</a> from pytest-dev/backport-12325-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2b671b5f9208650e8e42e07782d95477cc41f42a"><code>2b671b5</code></a> [8.2.x] cacheprovider: fix <code>.pytest_cache</code> not being world-readable</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/65ab7cb96c95f83e922f21bb4a8a44eda2b79707"><code>65ab7cb</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12324">#12324</a> from pytest-dev/backport-12320-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4d5fb7d71ccc069e2f882bee0e4253eaf484d2a9"><code>4d5fb7d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12319">#12319</a> from pytest-dev/backport-12311-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/cbe5996cc684b00397494d9590f3179de232c3ee"><code>cbe5996</code></a> [8.2.x] changelog: document unittest 8.2 change as breaking</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/537" class=".btn">#537</a>
            </td>
            <td>
                <b>
                    Bump pytest-asyncio from 0.23.6 to 0.23.7 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.6 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.6...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.6&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/536" class=".btn">#536</a>
            </td>
            <td>
                <b>
                    Bump pytest-asyncio from 0.23.6 to 0.23.7 in /rpc/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.6 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.6...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.6&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/535" class=".btn">#535</a>
            </td>
            <td>
                <b>
                    Bump node from 18 to 22 in /oid4vci/integration/afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps node from 18 to 22.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node&package-manager=docker&previous-version=18&new-version=22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/534" class=".btn">#534</a>
            </td>
            <td>
                <b>
                    Bump pytest-asyncio from 0.23.6 to 0.23.7 in /multitenant_provider/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.6 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.6...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.6&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/533" class=".btn">#533</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-bullseye to 3.12-bullseye in /plugin_globals/docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-bullseye to 3.12-bullseye.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-bullseye&new-version=3.12-bullseye)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/532" class=".btn">#532</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.1 in /firebase_push_notifications/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/66ff8dffdf9eee9b3dd6686de34542c49ff80dcd"><code>66ff8df</code></a> Prepare release version 8.2.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3ffcfd122cf4674ac45f6233d9b50be6c49abeea"><code>3ffcfd1</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12340">#12340</a> from pytest-dev/backport-12334-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0b28313b46a04de08bddc18896b3e61312a0c5b3"><code>0b28313</code></a> [8.2.x] Add Python 3.13 (beta) support</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f3dd93ad8d62eb0a260d3090f31be82aafbcff13"><code>f3dd93a</code></a> [8.2.x] Attest package provenance (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12335">#12335</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bb5a1257b0aafe5932377fa8e9fd92ab39418ac7"><code>bb5a125</code></a> [8.2.x] Spelling (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12331">#12331</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f179bf252fe2c1d0afce64b4b4bab4449e366e84"><code>f179bf2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12327">#12327</a> from pytest-dev/backport-12325-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2b671b5f9208650e8e42e07782d95477cc41f42a"><code>2b671b5</code></a> [8.2.x] cacheprovider: fix <code>.pytest_cache</code> not being world-readable</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/65ab7cb96c95f83e922f21bb4a8a44eda2b79707"><code>65ab7cb</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12324">#12324</a> from pytest-dev/backport-12320-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4d5fb7d71ccc069e2f882bee0e4253eaf484d2a9"><code>4d5fb7d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12319">#12319</a> from pytest-dev/backport-12311-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/cbe5996cc684b00397494d9590f3179de232c3ee"><code>cbe5996</code></a> [8.2.x] changelog: document unittest 8.2 change as breaking</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/531" class=".btn">#531</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-slim to 3.12-slim in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-slim to 3.12-slim.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-slim&new-version=3.12-slim)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/530" class=".btn">#530</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.1 in /basicmessage_storage/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/66ff8dffdf9eee9b3dd6686de34542c49ff80dcd"><code>66ff8df</code></a> Prepare release version 8.2.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3ffcfd122cf4674ac45f6233d9b50be6c49abeea"><code>3ffcfd1</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12340">#12340</a> from pytest-dev/backport-12334-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0b28313b46a04de08bddc18896b3e61312a0c5b3"><code>0b28313</code></a> [8.2.x] Add Python 3.13 (beta) support</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f3dd93ad8d62eb0a260d3090f31be82aafbcff13"><code>f3dd93a</code></a> [8.2.x] Attest package provenance (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12335">#12335</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bb5a1257b0aafe5932377fa8e9fd92ab39418ac7"><code>bb5a125</code></a> [8.2.x] Spelling (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12331">#12331</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f179bf252fe2c1d0afce64b4b4bab4449e366e84"><code>f179bf2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12327">#12327</a> from pytest-dev/backport-12325-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2b671b5f9208650e8e42e07782d95477cc41f42a"><code>2b671b5</code></a> [8.2.x] cacheprovider: fix <code>.pytest_cache</code> not being world-readable</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/65ab7cb96c95f83e922f21bb4a8a44eda2b79707"><code>65ab7cb</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12324">#12324</a> from pytest-dev/backport-12320-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4d5fb7d71ccc069e2f882bee0e4253eaf484d2a9"><code>4d5fb7d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12319">#12319</a> from pytest-dev/backport-12311-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/cbe5996cc684b00397494d9590f3179de232c3ee"><code>cbe5996</code></a> [8.2.x] changelog: document unittest 8.2 change as breaking</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/529" class=".btn">#529</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-bullseye to 3.12-bullseye in /rpc/docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-bullseye to 3.12-bullseye.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-bullseye&new-version=3.12-bullseye)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/528" class=".btn">#528</a>
            </td>
            <td>
                <b>
                    Bump react-bootstrap from 2.9.1 to 2.10.2 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react-bootstrap](https://github.com/react-bootstrap/react-bootstrap) from 2.9.1 to 2.10.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/react-bootstrap/react-bootstrap/releases">react-bootstrap's releases</a>.</em></p>
<blockquote>
<h2>v2.10.2</h2>
<h2><a href="https://github.com/react-bootstrap/react-bootstrap/compare/v2.10.1...v2.10.2">2.10.2</a> (2024-03-18)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>update <code>@​restart/ui</code> to v1.6.8 (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6779">#6779</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/c86187fe0426109fda9af4eac998d855645c1ee9">c86187f</a>)</li>
<li><strong>Tabs:</strong> add id attribute to nav (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6767">#6767</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/3b4fd9b83985efe97e8895fbe6d99db8548cd246">3b4fd9b</a>)</li>
</ul>
<h2>v2.10.1</h2>
<h2><a href="https://github.com/react-bootstrap/react-bootstrap/compare/v2.10.0...v2.10.1">2.10.1</a> (2024-02-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>FormControl:</strong> ensures compatibility with <code>@​types/react</code><a href="https://github.com/18"><code>@​18</code></a>.2.48 (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6763">#6763</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/652e709fe6f3b383e041474f776855431fc8e1ea">652e709</a>)</li>
</ul>
<h2>v2.10.0</h2>
<h1><a href="https://github.com/react-bootstrap/react-bootstrap/compare/v2.9.2...v2.10.0">2.10.0</a> (2024-01-17)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>Modal:</strong> properly handle <code>data-bs-theme</code> attribute (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6743">#6743</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/1ead9cac8a617c401a33fa921529d57e56db0718">1ead9ca</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li><strong>PageItem:</strong> implement &quot;as&quot; property (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6754">#6754</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/430b0c9589b76d89496b49a5cbdeaa38b9f828a0">430b0c9</a>)</li>
</ul>
<h2>v2.9.2</h2>
<h2><a href="https://github.com/react-bootstrap/react-bootstrap/compare/v2.9.1...v2.9.2">2.9.2</a> (2023-12-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>AccordionBody:</strong> add AccordionBody to index exports (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6732">#6732</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/d34244b9ed01eba003699b2a9b7d4228052640cb">d34244b</a>)</li>
<li><strong>Dropdown:</strong> prevent flickering on 'mousedown' rootCloseEvent (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6714">#6714</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/a58a0cd6e548c653cda23ed529f3cff69ec123cc">a58a0cd</a>)</li>
<li><strong>Navbar:</strong> add missing type for sticky bottom (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6726">#6726</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/36d0b7a92f9443d856f69b2d8cfbef1b868036c4">36d0b7a</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/react-bootstrap/react-bootstrap/blob/master/CHANGELOG.md">react-bootstrap's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/react-bootstrap/react-bootstrap/compare/v2.10.1...v2.10.2">2.10.2</a> (2024-03-18)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>update <code>@​restart/ui</code> to v1.6.8 (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6779">#6779</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/c86187fe0426109fda9af4eac998d855645c1ee9">c86187f</a>)</li>
<li><strong>Tabs:</strong> add id attribute to nav (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6767">#6767</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/3b4fd9b83985efe97e8895fbe6d99db8548cd246">3b4fd9b</a>)</li>
</ul>
<h2><a href="https://github.com/react-bootstrap/react-bootstrap/compare/v2.10.0...v2.10.1">2.10.1</a> (2024-02-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>FormControl:</strong> ensures compatibility with <code>@​types/react</code><a href="https://github.com/18"><code>@​18</code></a>.2.48 (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6763">#6763</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/652e709fe6f3b383e041474f776855431fc8e1ea">652e709</a>)</li>
</ul>
<h1><a href="https://github.com/react-bootstrap/react-bootstrap/compare/v2.9.2...v2.10.0">2.10.0</a> (2024-01-17)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>Modal:</strong> properly handle <code>data-bs-theme</code> attribute (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6743">#6743</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/1ead9cac8a617c401a33fa921529d57e56db0718">1ead9ca</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li><strong>PageItem:</strong> implement &quot;as&quot; property (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6754">#6754</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/430b0c9589b76d89496b49a5cbdeaa38b9f828a0">430b0c9</a>)</li>
</ul>
<h2><a href="https://github.com/react-bootstrap/react-bootstrap/compare/v2.9.1...v2.9.2">2.9.2</a> (2023-12-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>AccordionBody:</strong> add AccordionBody to index exports (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6732">#6732</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/d34244b9ed01eba003699b2a9b7d4228052640cb">d34244b</a>)</li>
<li><strong>Dropdown:</strong> prevent flickering on 'mousedown' rootCloseEvent (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6714">#6714</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/a58a0cd6e548c653cda23ed529f3cff69ec123cc">a58a0cd</a>)</li>
<li><strong>Navbar:</strong> add missing type for sticky bottom (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6726">#6726</a>) (<a href="https://github.com/react-bootstrap/react-bootstrap/commit/36d0b7a92f9443d856f69b2d8cfbef1b868036c4">36d0b7a</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/d005307790160f6e06dd8e771b88c799b433a2c2"><code>d005307</code></a> Publish v2.10.2</li>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/c86187fe0426109fda9af4eac998d855645c1ee9"><code>c86187f</code></a> fix: update <code>@​restart/ui</code> to v1.6.8 (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6779">#6779</a>)</li>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/522fd86af4d3204d8ab32c104d00cc77f483602c"><code>522fd86</code></a> chore: remove enzyme (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6777">#6777</a>)</li>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/d139e15a936ce07e4011d0d101807ef042a3b622"><code>d139e15</code></a> chore(ci): update to node 20 (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6774">#6774</a>)</li>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/3b4fd9b83985efe97e8895fbe6d99db8548cd246"><code>3b4fd9b</code></a> fix(Tabs): add id attribute to nav (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6767">#6767</a>)</li>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/346cb32bd8ab0a9d2a7ddd53de6cc5992914eb27"><code>346cb32</code></a> chore(ci): fix failing firefox tests (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6773">#6773</a>)</li>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/8c623894c6d387c8288d5a3c3d5bcbe9ecf47dd7"><code>8c62389</code></a> Publish v2.10.1</li>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/652e709fe6f3b383e041474f776855431fc8e1ea"><code>652e709</code></a> fix(FormControl): ensures compatibility with <code>@​types/react</code><a href="https://github.com/18"><code>@​18</code></a>.2.48 (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6763">#6763</a>)</li>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/88334cfcf15894f81a113a5856fe6c96ce92489c"><code>88334cf</code></a> docs: rollback react-docgen (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6765">#6765</a>)</li>
<li><a href="https://github.com/react-bootstrap/react-bootstrap/commit/35982cadf2c909611c104f448a8603aa96a88734"><code>35982ca</code></a> docs: update to Docusaurus v3 (<a href="https://redirect.github.com/react-bootstrap/react-bootstrap/issues/6756">#6756</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/react-bootstrap/react-bootstrap/compare/v2.9.1...v2.10.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-bootstrap&package-manager=npm_and_yarn&previous-version=2.9.1&new-version=2.10.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/527" class=".btn">#527</a>
            </td>
            <td>
                <b>
                    Bump uvicorn from 0.15.0 to 0.16.0 in /kafka_events/kafka_events/v1_0/http_kafka_relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [uvicorn](https://github.com/encode/uvicorn) from 0.15.0 to 0.16.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/encode/uvicorn/releases">uvicorn's releases</a>.</em></p>
<blockquote>
<h2>Version 0.16.0</h2>
<h2>0.16.0 - 2021-12-08</h2>
<h3>Added</h3>
<ul>
<li>Enable read of uvicorn settings from environment variables (<a href="https://redirect.github.com/encode/uvicorn/issues/1279">#1279</a>) 06/12/21</li>
<li>Bump <code>websockets</code> to 10.0. (<a href="https://redirect.github.com/encode/uvicorn/issues/1180">#1180</a>) 13/09/21</li>
<li>Ensure non-zero exit code when startup fails (<a href="https://redirect.github.com/encode/uvicorn/issues/1278">#1278</a>) 06/12/21</li>
<li>Increase <code>httptools</code> version range from &quot;==0.2.*&quot; to &quot;&gt;=0.2.0,&lt;0.4.0&quot;. (<a href="https://redirect.github.com/encode/uvicorn/issues/1243">#1243</a>) 8/11/21</li>
<li>Override default asyncio event loop with reload only on Windows (<a href="https://redirect.github.com/encode/uvicorn/issues/1257">#1257</a>) 24/11/21</li>
<li>Replace <code>HttpToolsProtocol.pipeline</code> type from <code>list</code> to <code>deque</code>. (<a href="https://redirect.github.com/encode/uvicorn/issues/1213">#1213</a>) 10/10/21</li>
<li>Replace <code>WSGIResponder.send_queue</code> type from <code>list</code> to <code>deque</code>. (<a href="https://redirect.github.com/encode/uvicorn/issues/1214">#1214</a>) 10/10/21</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Main process exit after startup failure on reloader classes (<a href="https://redirect.github.com/encode/uvicorn/issues/1177">#1177</a>) 30/09/21</li>
<li>Add explicit casting on click options (<a href="https://redirect.github.com/encode/uvicorn/issues/1217">#1217</a>) 11/10/21</li>
<li>Allow WebSocket close event to receive reason being None from ASGI app. (<a href="https://redirect.github.com/encode/uvicorn/issues/1259">#1259</a>) 23/11/21</li>
<li>Fix a bug in <code>WebSocketProtocol.asgi_receive</code> on which we returned a close frame even if there were data messages before that frame in the read queue. (<a href="https://redirect.github.com/encode/uvicorn/issues/1252">#1252</a>) 25/11/21</li>
<li>The option <code>--reload-dirs</code> was splitting a string into single character directories. (<a href="https://redirect.github.com/encode/uvicorn/issues/1267">#1267</a>) 25/11/21</li>
<li>Only second SIGINT is able to forcelly shutdown the server (<a href="https://redirect.github.com/encode/uvicorn/issues/1269">#1269</a>) 28/11/21</li>
<li>Allow app-dir parameter on the run() function (<a href="https://redirect.github.com/encode/uvicorn/issues/1271">#1271</a>) 06/12/21</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/encode/uvicorn/blob/master/CHANGELOG.md">uvicorn's changelog</a>.</em></p>
<blockquote>
<h2>0.16.0 (2021-12-08)</h2>
<h3>Added</h3>
<ul>
<li>Enable read of uvicorn settings from environment variables (<a href="https://redirect.github.com/encode/uvicorn/issues/1279">#1279</a>)</li>
<li>Bump <code>websockets</code> to 10.0. (<a href="https://redirect.github.com/encode/uvicorn/issues/1180">#1180</a>)</li>
<li>Ensure non-zero exit code when startup fails (<a href="https://redirect.github.com/encode/uvicorn/issues/1278">#1278</a>)</li>
<li>Increase <code>httptools</code> version range from &quot;==0.2.*&quot; to &quot;&gt;=0.2.0,&lt;0.4.0&quot;. (<a href="https://redirect.github.com/encode/uvicorn/issues/1243">#1243</a>)</li>
<li>Override default asyncio event loop with reload only on Windows (<a href="https://redirect.github.com/encode/uvicorn/issues/1257">#1257</a>)</li>
<li>Replace <code>HttpToolsProtocol.pipeline</code> type from <code>list</code> to <code>deque</code>. (<a href="https://redirect.github.com/encode/uvicorn/issues/1213">#1213</a>)</li>
<li>Replace <code>WSGIResponder.send_queue</code> type from <code>list</code> to <code>deque</code>. (<a href="https://redirect.github.com/encode/uvicorn/issues/1214">#1214</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Main process exit after startup failure on reloader classes (<a href="https://redirect.github.com/encode/uvicorn/issues/1177">#1177</a>)</li>
<li>Add explicit casting on click options (<a href="https://redirect.github.com/encode/uvicorn/issues/1217">#1217</a>)</li>
<li>Allow WebSocket close event to receive reason being None from ASGI app. (<a href="https://redirect.github.com/encode/uvicorn/issues/1259">#1259</a>)</li>
<li>Fix a bug in <code>WebSocketProtocol.asgi_receive</code> on which we returned a close frame even if there were data messages before that frame in the read queue. (<a href="https://redirect.github.com/encode/uvicorn/issues/1252">#1252</a>)</li>
<li>The option <code>--reload-dirs</code> was splitting a string into single character directories. (<a href="https://redirect.github.com/encode/uvicorn/issues/1267">#1267</a>)</li>
<li>Only second SIGINT is able to forcefully shutdown the server (<a href="https://redirect.github.com/encode/uvicorn/issues/1269">#1269</a>)</li>
<li>Allow app-dir parameter on the run() function (<a href="https://redirect.github.com/encode/uvicorn/issues/1271">#1271</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/encode/uvicorn/commit/65ec8d132c37a8338a2f495fa1be9f14bd4368d9"><code>65ec8d1</code></a> Version 0.16.0 (<a href="https://redirect.github.com/encode/uvicorn/issues/1270">#1270</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/edb645468b6082b95bb3a173c2e8a24c8b083c67"><code>edb6454</code></a> Allow app-dir parameter on the run() function (<a href="https://redirect.github.com/encode/uvicorn/issues/1271">#1271</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/9c1b88c0a76d600359af0c87825799115d75ded5"><code>9c1b88c</code></a> Enable read of uvicorn settings from environment variables (<a href="https://redirect.github.com/encode/uvicorn/issues/1279">#1279</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/825aeba513ce434a77bbcbce356cc788d150445f"><code>825aeba</code></a> Ensure non-zero exit code when startup fails (<a href="https://redirect.github.com/encode/uvicorn/issues/1278">#1278</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/63a10e57d43340f3dc25bd29f45ecd5f75c75ed8"><code>63a10e5</code></a> Update GitHub templates with new forms (<a href="https://redirect.github.com/encode/uvicorn/issues/1280">#1280</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/ecd2cc721851788c463b7e4e8b1772193a762439"><code>ecd2cc7</code></a> Only second SIGINT is able to forcelly shutdown the server (<a href="https://redirect.github.com/encode/uvicorn/issues/1269">#1269</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/d3e6fc948391923a1c74d8e0a1344e1a50b5ea75"><code>d3e6fc9</code></a> fix reload_dirs (<a href="https://redirect.github.com/encode/uvicorn/issues/1267">#1267</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/5478e71c2d14ff0cad3d726daa38acffd9f6c972"><code>5478e71</code></a> Fixed a bug in asgi_receive that returned a close frame even if there were da...</li>
<li><a href="https://github.com/encode/uvicorn/commit/81802ceee2a2c62f0b10f78e2b6366b47bc76f72"><code>81802ce</code></a> Override default asyncio event loop with reload only on Windows (<a href="https://redirect.github.com/encode/uvicorn/issues/1257">#1257</a>)</li>
<li><a href="https://github.com/encode/uvicorn/commit/0dcfc0227d6dbc0feaaf215e778d83b5a2895423"><code>0dcfc02</code></a> Add contributing page to the docs (<a href="https://redirect.github.com/encode/uvicorn/issues/1197">#1197</a>) (<a href="https://redirect.github.com/encode/uvicorn/issues/1224">#1224</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/encode/uvicorn/compare/0.15.0...0.16.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uvicorn&package-manager=pip&previous-version=0.15.0&new-version=0.16.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/526" class=".btn">#526</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-bullseye to 3.12-bullseye in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-bullseye to 3.12-bullseye.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-bullseye&new-version=3.12-bullseye)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/525" class=".btn">#525</a>
            </td>
            <td>
                <b>
                    Bump aiokafka from 0.7.2 to 0.10.0 in /kafka_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aiokafka](https://github.com/aio-libs/aiokafka) from 0.7.2 to 0.10.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiokafka/releases">aiokafka's releases</a>.</em></p>
<blockquote>
<h2>v0.10.0</h2>
<p>New features:</p>
<ul>
<li>Support static membership protocol, <a href="https://cwiki.apache.org/confluence/display/KAFKA/KIP-345%3A+Introduce+static+membership+protocol+to+reduce+consumer+rebalances">KIP-345</a> (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/680">#680</a>, pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/941">#941</a> by
<a href="https://github.com/patkivikram"><code>@​patkivikram</code></a> and <a href="https://github.com/joshuaherrera"><code>@​joshuaherrera</code></a>)</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Fix extra dependencies (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/952">#952</a>)</li>
</ul>
<h2>v0.10.0.a0</h2>
<p>New features:</p>
<ul>
<li>Support static membership protocol, <a href="https://cwiki.apache.org/confluence/display/KAFKA/KIP-345%3A+Introduce+static+membership+protocol+to+reduce+consumer+rebalances">KIP-345</a> (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/680">#680</a>, pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/941">#941</a> by
<a href="https://github.com/patkivikram"><code>@​patkivikram</code></a> and <a href="https://github.com/joshuaherrera"><code>@​joshuaherrera</code></a>)</li>
</ul>
<h2>v0.9.0</h2>
<p>New features:</p>
<ul>
<li>Include <code>kafka-python</code> into <code>aiokafka</code>'s code base (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/928">#928</a> and others)</li>
<li>Replace <code>python-snappy</code> and <code>zstandard</code> with <code>cramjam</code> (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/930">#930</a>)</li>
<li>PEP518 compliant <code>pyproject.toml</code></li>
<li>Python 3.12 support</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Fix type annotation for <code>ConsumerRecord</code> (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/912">#912</a> by <a href="https://github.com/zschumacher"><code>@​zschumacher</code></a>)</li>
<li>Improve send performance (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/943">#943</a>)</li>
</ul>
<p>Improved Documentation:</p>
<ul>
<li>Fix <code>AbstractTokenProvider.token</code> example (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/919">#919</a> by <a href="https://github.com/mtomilov"><code>@​mtomilov</code></a>)</li>
</ul>
<h2>v0.9.0.rc1</h2>
<p>New features:</p>
<ul>
<li>Include <code>kafka-python</code> into <code>aiokafka</code>'s code base</li>
<li>Replace <code>python-snappy</code> and <code>zstandard</code> with <code>cramjam</code></li>
<li>PEP518 compliant <code>pyproject.toml</code></li>
<li>Python 3.12 support</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Fix type annotation for <code>ConsumerRecord</code> (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/912">#912</a> by <a href="https://github.com/zschumacher"><code>@​zschumacher</code></a>)</li>
<li>Improve send performance (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/943">#943</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiokafka/blob/master/CHANGES.rst">aiokafka's changelog</a>.</em></p>
<blockquote>
<h1>0.10.0 (2023-12-15)</h1>
<p>New features:</p>
<ul>
<li>Support static membership protocol, <code>KIP-345</code>_ (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/680">#680</a>, pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/941">#941</a> by
<a href="https://github.com/patkivikram"><code>@​patkivikram</code></a> and <a href="https://github.com/joshuaherrera"><code>@​joshuaherrera</code></a>)</li>
</ul>
<p>.. _KIP-345: <a href="https://cwiki.apache.org/confluence/display/KAFKA/KIP-345%3A+Introduce+static+membership+protocol+to+reduce+consumer+rebalances">https://cwiki.apache.org/confluence/display/KAFKA/KIP-345%3A+Introduce+static+membership+protocol+to+reduce+consumer+rebalances</a></p>
<p>Bugfixes:</p>
<ul>
<li>Fix extra dependencies (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/952">#952</a>)</li>
</ul>
<h1>0.9.0 (2023-12-04)</h1>
<p>New features:</p>
<ul>
<li>Include <code>kafka-python</code> into <code>aiokafka</code>'s code base (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/928">#928</a> and others)</li>
<li>Replace <code>python-snappy</code> and <code>zstandard</code> with <code>cramjam</code> (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/930">#930</a>)</li>
<li>PEP518 compliant <code>pyproject.toml</code></li>
<li>Python 3.12 support</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Fix type annotation for <code>ConsumerRecord</code> (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/912">#912</a> by <a href="https://github.com/zschumacher"><code>@​zschumacher</code></a>)</li>
<li>Improve send performance (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/943">#943</a>)</li>
<li>Fix <code>DescribeConfigsResponse_v1</code></li>
</ul>
<p>Improved Documentation:</p>
<ul>
<li>Fix <code>AbstractTokenProvider.token</code> example (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/919">#919</a> by <a href="https://github.com/mtomilov"><code>@​mtomilov</code></a>)</li>
</ul>
<h1>0.8.1 (2023-05-31)</h1>
<p>New features:</p>
<ul>
<li>Drop support for Python 3.7 due to end of life (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/893">#893</a>)</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Add SASL authentication support to <code>AIOKafkaAdminClient</code> (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/889">#889</a>,</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiokafka/commit/85f758e1833e012b87e84a7ef5d81394a7b15acb"><code>85f758e</code></a> Prepare 0.10.0 release</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/7073b09b4a3f32a6e08e676327f85be6a36e5412"><code>7073b09</code></a> Fix optional dependencies (<a href="https://redirect.github.com/aio-libs/aiokafka/issues/952">#952</a>) (<a href="https://redirect.github.com/aio-libs/aiokafka/issues/953">#953</a>)</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/7ea1bea1298d913c71b7f506adcfdb42774dae5b"><code>7ea1bea</code></a> Prepare 0.10.0.a0 release</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/7b6c94e43b4a96fe7ebf2e7ac23c30d9b421d684"><code>7b6c94e</code></a> Add CodeQL workflow (<a href="https://redirect.github.com/aio-libs/aiokafka/issues/864">#864</a>)</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/b1a3dfcd7732bc7c6dc5fd63d0b94f3748699932"><code>b1a3dfc</code></a> Update consumer.rst documentation for correct ordering of consumer subscripti...</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/bc14e6daa3aa92c7dd39b448e1dc7ff0807579ad"><code>bc14e6d</code></a> Implement KIP-345 in aiokafka (rebase of <a href="https://redirect.github.com/aio-libs/aiokafka/issues/827">#827</a>) (<a href="https://redirect.github.com/aio-libs/aiokafka/issues/941">#941</a>)</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/881851783673e927591ba274a7703c9b52d387ac"><code>8818517</code></a> Prepare 0.9.0 release</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/d7201c1e26fd2f3e51f15a2cdeda9753d4fd3a1a"><code>d7201c1</code></a> Prepare 0.9.0.rc1 release</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/a25e5c2294ab5967dc4480a71dd07244cbca468d"><code>a25e5c2</code></a> Merge pull request <a href="https://redirect.github.com/aio-libs/aiokafka/issues/947">#947</a> from ods/kafka-python-cleanup</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/fdba76455bfeb91ec349201e396e9840ddda2f90"><code>fdba764</code></a> Fix docstrings</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiokafka/compare/v0.7.2...v0.10.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiokafka&package-manager=pip&previous-version=0.7.2&new-version=0.10.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/522" class=".btn">#522</a>
            </td>
            <td>
                <b>
                    Bump requests from 2.32.0 to 2.32.2 in /rpc/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.32.0 to 2.32.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.2</h2>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>v2.32.1</h2>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li><a href="https://github.com/psf/requests/commit/970e8cec988421bd43da57350723b05c8ce8dc7e"><code>970e8ce</code></a> v2.32.1</li>
<li>See full diff in <a href="https://github.com/psf/requests/compare/v2.32.0...v2.32.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.32.0&new-version=2.32.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/521" class=".btn">#521</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.1 in /connection_update/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/66ff8dffdf9eee9b3dd6686de34542c49ff80dcd"><code>66ff8df</code></a> Prepare release version 8.2.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3ffcfd122cf4674ac45f6233d9b50be6c49abeea"><code>3ffcfd1</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12340">#12340</a> from pytest-dev/backport-12334-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0b28313b46a04de08bddc18896b3e61312a0c5b3"><code>0b28313</code></a> [8.2.x] Add Python 3.13 (beta) support</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f3dd93ad8d62eb0a260d3090f31be82aafbcff13"><code>f3dd93a</code></a> [8.2.x] Attest package provenance (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12335">#12335</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bb5a1257b0aafe5932377fa8e9fd92ab39418ac7"><code>bb5a125</code></a> [8.2.x] Spelling (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12331">#12331</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f179bf252fe2c1d0afce64b4b4bab4449e366e84"><code>f179bf2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12327">#12327</a> from pytest-dev/backport-12325-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2b671b5f9208650e8e42e07782d95477cc41f42a"><code>2b671b5</code></a> [8.2.x] cacheprovider: fix <code>.pytest_cache</code> not being world-readable</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/65ab7cb96c95f83e922f21bb4a8a44eda2b79707"><code>65ab7cb</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12324">#12324</a> from pytest-dev/backport-12320-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4d5fb7d71ccc069e2f882bee0e4253eaf484d2a9"><code>4d5fb7d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12319">#12319</a> from pytest-dev/backport-12311-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/cbe5996cc684b00397494d9590f3179de232c3ee"><code>cbe5996</code></a> [8.2.x] changelog: document unittest 8.2 change as breaking</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/519" class=".btn">#519</a>
            </td>
            <td>
                <b>
                    Bump requests from 2.32.0 to 2.32.2 in /multitenant_provider/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.32.0 to 2.32.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.2</h2>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>v2.32.1</h2>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li><a href="https://github.com/psf/requests/commit/970e8cec988421bd43da57350723b05c8ce8dc7e"><code>970e8ce</code></a> v2.32.1</li>
<li>See full diff in <a href="https://github.com/psf/requests/compare/v2.32.0...v2.32.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.32.0&new-version=2.32.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/517" class=".btn">#517</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-slim to 3.12-slim in /rpc/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-slim to 3.12-slim.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-slim&new-version=3.12-slim)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/515" class=".btn">#515</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.1 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/66ff8dffdf9eee9b3dd6686de34542c49ff80dcd"><code>66ff8df</code></a> Prepare release version 8.2.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3ffcfd122cf4674ac45f6233d9b50be6c49abeea"><code>3ffcfd1</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12340">#12340</a> from pytest-dev/backport-12334-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0b28313b46a04de08bddc18896b3e61312a0c5b3"><code>0b28313</code></a> [8.2.x] Add Python 3.13 (beta) support</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f3dd93ad8d62eb0a260d3090f31be82aafbcff13"><code>f3dd93a</code></a> [8.2.x] Attest package provenance (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12335">#12335</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bb5a1257b0aafe5932377fa8e9fd92ab39418ac7"><code>bb5a125</code></a> [8.2.x] Spelling (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12331">#12331</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f179bf252fe2c1d0afce64b4b4bab4449e366e84"><code>f179bf2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12327">#12327</a> from pytest-dev/backport-12325-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2b671b5f9208650e8e42e07782d95477cc41f42a"><code>2b671b5</code></a> [8.2.x] cacheprovider: fix <code>.pytest_cache</code> not being world-readable</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/65ab7cb96c95f83e922f21bb4a8a44eda2b79707"><code>65ab7cb</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12324">#12324</a> from pytest-dev/backport-12320-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4d5fb7d71ccc069e2f882bee0e4253eaf484d2a9"><code>4d5fb7d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12319">#12319</a> from pytest-dev/backport-12311-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/cbe5996cc684b00397494d9590f3179de232c3ee"><code>cbe5996</code></a> [8.2.x] changelog: document unittest 8.2 change as breaking</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/514" class=".btn">#514</a>
            </td>
            <td>
                <b>
                    Bump react-router-dom from 6.16.0 to 6.23.1 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react-router-dom](https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom) from 6.16.0 to 6.23.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/remix-run/react-router/releases">react-router-dom's releases</a>.</em></p>
<blockquote>
<h2>react-router-dom-v5-compat@6.4.0-pre.15</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.15</li>
<li>react-router-dom@6.4.0-pre.15</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.11</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.11</li>
<li>react-router-dom@6.4.0-pre.11</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.10</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.10</li>
<li>react-router-dom@6.4.0-pre.10</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.9</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.9</li>
<li>react-router-dom@6.4.0-pre.9</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.8</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li>react-router@6.4.0-pre.8</li>
<li>react-router-dom@6.4.0-pre.8</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.7</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies
<ul>
<li><code>react-router@6.4.0-pre.7</code></li>
<li><code>react-router-dom@6.4.0-pre.7</code></li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.6</h2>
<h3>Patch Changes</h3>
<ul>
<li>44bce3c6: Fix <code>react-router-dom</code> peer dependency version
<ul>
<li>react-router@6.4.0-pre.6</li>
<li>react-router-dom@6.4.0-pre.6</li>
</ul>
</li>
</ul>
<h2>react-router-dom-v5-compat@6.4.0-pre.5</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/remix-run/react-router/blob/main/packages/react-router-dom/CHANGELOG.md">react-router-dom's changelog</a>.</em></p>
<blockquote>
<h2>6.23.1</h2>
<h3>Patch Changes</h3>
<ul>
<li>Check for <code>document</code> existence when checking <code>startViewTransition</code> (<a href="https://redirect.github.com/remix-run/react-router/pull/11544">#11544</a>)</li>
<li>Change the <code>react-router-dom/server</code> import back to <code>react-router-dom</code> instead of <code>index.ts</code> (<a href="https://redirect.github.com/remix-run/react-router/pull/11514">#11514</a>)</li>
<li>Updated dependencies:
<ul>
<li><code>@remix-run/router@1.16.1</code></li>
<li><code>react-router@6.23.1</code></li>
</ul>
</li>
</ul>
<h2>6.23.0</h2>
<h3>Minor Changes</h3>
<ul>
<li>Add a new <code>unstable_dataStrategy</code> configuration option (<a href="https://redirect.github.com/remix-run/react-router/pull/11098">#11098</a>)
<ul>
<li>This option allows Data Router applications to take control over the approach for executing route loaders and actions</li>
<li>The default implementation is today's behavior, to fetch all loaders in parallel, but this option allows users to implement more advanced data flows including Remix single-fetch, middleware/context APIs, automatic loader caching, and more</li>
</ul>
</li>
</ul>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies:
<ul>
<li><code>@remix-run/router@1.16.0</code></li>
<li><code>react-router@6.23.0</code></li>
</ul>
</li>
</ul>
<h2>6.22.3</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies:
<ul>
<li><code>@remix-run/router@1.15.3</code></li>
<li><code>react-router@6.22.3</code></li>
</ul>
</li>
</ul>
<h2>6.22.2</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies:
<ul>
<li><code>@remix-run/router@1.15.2</code></li>
<li><code>react-router@6.22.2</code></li>
</ul>
</li>
</ul>
<h2>6.22.1</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies:
<ul>
<li><code>react-router@6.22.1</code></li>
<li><code>@remix-run/router@1.15.1</code></li>
</ul>
</li>
</ul>
<h2>6.22.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/remix-run/react-router/commit/aef5c4a617756e6fcc493de17b4be9997a5a19c8"><code>aef5c4a</code></a> chore: Update version for release (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11551">#11551</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/26bc8e295398b571104ef529149c22a0724eeb7e"><code>26bc8e2</code></a> chore: Update version for release (pre) (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11545">#11545</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/031478d4acc46cc631673ef14e3215fac97dee8b"><code>031478d</code></a> Add defensive window.document check when checking for startViewTransition (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/1">#1</a>...</li>
<li><a href="https://github.com/remix-run/react-router/commit/9651465485fc6c96c1dd793a96d8af8f1ebf42d0"><code>9651465</code></a> chore: Update version for release (pre) (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11516">#11516</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/fdff9ddfd3b929b6750f750523b77649d1421e60"><code>fdff9dd</code></a> Fix react-router-dom/server index.ts import from pnpm migration (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11514">#11514</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/82a3a778b23ed991fb71e6f188bb7d06cc3c7d62"><code>82a3a77</code></a> chore: Update version for release (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11486">#11486</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/8a20f324602afa7b867b5c218c919cc041f21c49"><code>8a20f32</code></a> chore: Update version for release (pre) (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11387">#11387</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/88ec71a6d4159500cfbc69412112b128c669040a"><code>88ec71a</code></a> chore: Update version for release (pre) (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11379">#11379</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/12afb2efdc8408bd9e87e03f8fd16dd21ef1b233"><code>12afb2e</code></a> Migrate to pnpm (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11358">#11358</a>)</li>
<li><a href="https://github.com/remix-run/react-router/commit/c7dd3d3a8e00e96a238801d0fa00d24989cc4270"><code>c7dd3d3</code></a> Data Strategy Configuration (<a href="https://github.com/remix-run/react-router/tree/HEAD/packages/react-router-dom/issues/11098">#11098</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/remix-run/react-router/commits/react-router-dom@6.23.1/packages/react-router-dom">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-router-dom&package-manager=npm_and_yarn&previous-version=6.16.0&new-version=6.23.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/513" class=".btn">#513</a>
            </td>
            <td>
                <b>
                    Bump pytest-asyncio from 0.23.6 to 0.23.7 in /basicmessage_storage/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.6 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.6...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.6&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/512" class=".btn">#512</a>
            </td>
            <td>
                <b>
                    Bump pytest-asyncio from 0.23.6 to 0.23.7 in /firebase_push_notifications/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.6 to 0.23.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.7</h2>
<h1>0.23.7 (2024-05-19)</h1>
<ul>
<li>Silence deprecation warnings about unclosed event loops that occurred with certain CPython patch releases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/817">#817</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/eb63d5ad0ca21041726ada3d5c00211d36418a9b"><code>eb63d5a</code></a> docs: Prepared for release of v0.23.7.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/da04a7a645bdd46d0533c727e85cf2c0e13c7def"><code>da04a7a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/00c667ad80571fc8e937f4422267b135f55ec6e6"><code>00c667a</code></a> Build(deps): Bump pytest from 8.1.1 to 8.2.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bd9cd885b5cc78ce4a73a03c878ac93e0a1840f"><code>3bd9cd8</code></a> [docs] Add changelog entry.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/15544f0ee29152086b14e63cb040836f33b0b416"><code>15544f0</code></a> Revert GitHub Actions and Tox changes.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6316b285c1ee8f6d300916e531ff1d320bec8d6b"><code>6316b28</code></a> Deduplicate simplefilter snippet.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3ffdfc5607a112a9a2cb933a6af044eaf47e0227"><code>3ffdfc5</code></a> asyncio.run(port_afinalizer())</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/0107fd7ae7e42d399b5be9af6f3ee4427e16ea7d"><code>0107fd7</code></a> Remove extra space.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3bf700a80cb12354fbe0a9295be9fbd4317c8d8f"><code>3bf700a</code></a> Fix GH Action mapping.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d15dc31f7459810af824b5e9e903f914140ceb2c"><code>d15dc31</code></a> Fix 3109/3108 typo.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.6...v0.23.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.6&new-version=0.23.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/511" class=".btn">#511</a>
            </td>
            <td>
                <b>
                    Bump fastapi from 0.68.2 to 0.83.0 in /kafka_events/kafka_events/v1_0/http_kafka_relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [fastapi](https://github.com/tiangolo/fastapi) from 0.68.2 to 0.83.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tiangolo/fastapi/releases">fastapi's releases</a>.</em></p>
<blockquote>
<h2>0.83.0</h2>
<p>🚨 This is probably the last release (or one of the last releases) to support Python 3.6. 🔥</p>
<p>Python 3.6 reached the <a href="https://www.python.org/downloads/release/python-3615/">end-of-life and is no longer supported by Python</a> since around a year ago.</p>
<p>You hopefully updated to a supported version of Python a while ago. If you haven't, you really should.</p>
<h3>Features</h3>
<ul>
<li>✨ Add support in <code>jsonable_encoder</code> for include and exclude with dataclasses. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/4923">#4923</a> by <a href="https://github.com/DCsunset"><code>@​DCsunset</code></a>.</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>🐛 Fix <code>RuntimeError</code> raised when <code>HTTPException</code> has a status code with no content. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5365">#5365</a> by <a href="https://github.com/iudeen"><code>@​iudeen</code></a>.</li>
<li>🐛 Fix empty reponse body when default <code>status_code</code> is empty but the a <code>Response</code> parameter with <code>response.status_code</code> is set. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5360">#5360</a> by <a href="https://github.com/tmeckel"><code>@​tmeckel</code></a>.</li>
</ul>
<h3>Docs</h3>
<ul>
<li>📝 Update <code>SECURITY.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5377">#5377</a> by <a href="https://github.com/Kludex"><code>@​Kludex</code></a>.</li>
</ul>
<h3>Internal</h3>
<ul>
<li>⬆ [pre-commit.ci] pre-commit autoupdate. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5352">#5352</a> by <a href="https://github.com/apps/pre-commit-ci"><code>@​pre-commit-ci[bot]</code></a>.</li>
</ul>
<h2>0.82.0</h2>
<p>🚨 This is probably the last release (or one of the last releases) to support Python 3.6. 🔥</p>
<p>Python 3.6 reached the <a href="https://www.python.org/downloads/release/python-3615/">end-of-life and is no longer supported by Python</a> since around a year ago.</p>
<p>You hopefully updated to a supported version of Python a while ago. If you haven't, you really should.</p>
<h3>Features</h3>
<ul>
<li>✨ Export <code>WebSocketState</code> in <code>fastapi.websockets</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/4376">#4376</a> by <a href="https://github.com/matiuszka"><code>@​matiuszka</code></a>.</li>
<li>✨ Support Python internal description on Pydantic model's docstring. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/3032">#3032</a> by <a href="https://github.com/Kludex"><code>@​Kludex</code></a>.</li>
<li>✨ Update <code>ORJSONResponse</code> to support non <code>str</code> keys and serializing Numpy arrays. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/3892">#3892</a> by <a href="https://github.com/baby5"><code>@​baby5</code></a>.</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>🐛 Allow exit code for dependencies with <code>yield</code> to always execute, by removing capacity limiter for them, to e.g. allow closing DB connections without deadlocks. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5122">#5122</a> by <a href="https://github.com/adriangb"><code>@​adriangb</code></a>.</li>
<li>🐛 Fix FastAPI People GitHub Action: set HTTPX timeout for GraphQL query request. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5222">#5222</a> by <a href="https://github.com/iudeen"><code>@​iudeen</code></a>.</li>
<li>🐛 Make sure a parameter defined as required is kept required in OpenAPI even if defined as optional in another dependency. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/4319">#4319</a> by <a href="https://github.com/cd17822"><code>@​cd17822</code></a>.</li>
<li>🐛 Fix support for path parameters in WebSockets. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/3879">#3879</a> by <a href="https://github.com/davidbrochart"><code>@​davidbrochart</code></a>.</li>
</ul>
<h3>Docs</h3>
<ul>
<li>✏ Update Hypercorn link, now pointing to GitHub. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5346">#5346</a> by <a href="https://github.com/baconfield"><code>@​baconfield</code></a>.</li>
<li>✏ Tweak wording in <code>docs/en/docs/advanced/dataclasses.md</code>. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/3698">#3698</a> by <a href="https://github.com/pfackeldey"><code>@​pfackeldey</code></a>.</li>
<li>📝 Add note about Python 3.10 <code>X | Y</code> operator in explanation about Response Models. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5307">#5307</a> by <a href="https://github.com/MendyLanda"><code>@​MendyLanda</code></a>.</li>
<li>📝 Add link to New Relic article: &quot;How to monitor FastAPI application performance using Python agent&quot;. PR <a href="https://redirect.github.com/tiangolo/fastapi/pull/5260">#5260</a> by <a href="https://github.com/sjyothi54"><code>@​sjyothi54</code></a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tiangolo/fastapi/commit/b2aa3593be300b57973987fb2489ed01ed9c9f68"><code>b2aa359</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/ed0fcba7cbea46b0cca74e9fce568f9c7316d8e8"><code>ed0fcba</code></a> 🔖 Release version 0.83.0</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/22a155efc1ba51b215ed0aedcc0054854e85122e"><code>22a155e</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/306326a2138eff3835901fa34190e4475aed1409"><code>306326a</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/4fec12b354c7d87101aac60d0143236afcd8678f"><code>4fec12b</code></a> 📝 Update <code>SECURITY.md</code> (<a href="https://redirect.github.com/tiangolo/fastapi/issues/5377">#5377</a>)</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/275306c369d7186aebf6e6d7d56be11e6d01c43c"><code>275306c</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/4d270463af2279d9723d99da45f0b31631424030"><code>4d27046</code></a> 🐛Fix <code>RuntimeError</code> raised when <code>HTTPException</code> has a status code with no con...</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/6620273083275f7fec446bb3456d3df6582c6813"><code>6620273</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/0b4fe10c8fed59de02100612a6168a9aefaf3659"><code>0b4fe10</code></a> 🐛 Fix empty reponse body when default <code>status_code</code> is empty but the a `Respo...</li>
<li><a href="https://github.com/tiangolo/fastapi/commit/c4007cb9ecacd54df95e29780976937af01ff5ae"><code>c4007cb</code></a> 📝 Update release notes</li>
<li>Additional commits viewable in <a href="https://github.com/tiangolo/fastapi/compare/0.68.2...0.83.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=fastapi&package-manager=pip&previous-version=0.68.2&new-version=0.83.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/510" class=".btn">#510</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-slim to 3.12-slim in /multitenant_provider/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-slim to 3.12-slim.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-slim&new-version=3.12-slim)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/509" class=".btn">#509</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-alpine to 3.12-alpine in /kafka_events/kafka_events/v1_0/deliverer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-alpine to 3.12-alpine.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-alpine&new-version=3.12-alpine)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/508" class=".btn">#508</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.1 in /kafka_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/66ff8dffdf9eee9b3dd6686de34542c49ff80dcd"><code>66ff8df</code></a> Prepare release version 8.2.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3ffcfd122cf4674ac45f6233d9b50be6c49abeea"><code>3ffcfd1</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12340">#12340</a> from pytest-dev/backport-12334-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0b28313b46a04de08bddc18896b3e61312a0c5b3"><code>0b28313</code></a> [8.2.x] Add Python 3.13 (beta) support</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f3dd93ad8d62eb0a260d3090f31be82aafbcff13"><code>f3dd93a</code></a> [8.2.x] Attest package provenance (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12335">#12335</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bb5a1257b0aafe5932377fa8e9fd92ab39418ac7"><code>bb5a125</code></a> [8.2.x] Spelling (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12331">#12331</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f179bf252fe2c1d0afce64b4b4bab4449e366e84"><code>f179bf2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12327">#12327</a> from pytest-dev/backport-12325-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2b671b5f9208650e8e42e07782d95477cc41f42a"><code>2b671b5</code></a> [8.2.x] cacheprovider: fix <code>.pytest_cache</code> not being world-readable</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/65ab7cb96c95f83e922f21bb4a8a44eda2b79707"><code>65ab7cb</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12324">#12324</a> from pytest-dev/backport-12320-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4d5fb7d71ccc069e2f882bee0e4253eaf484d2a9"><code>4d5fb7d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12319">#12319</a> from pytest-dev/backport-12311-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/cbe5996cc684b00397494d9590f3179de232c3ee"><code>cbe5996</code></a> [8.2.x] changelog: document unittest 8.2 change as breaking</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/507" class=".btn">#507</a>
            </td>
            <td>
                <b>
                    Bump async-selective-queue from 0.1.0.post0 to 0.1.1 in /oid4vci/integration/afj_runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [async-selective-queue](https://github.com/dbluhm/async-selective-queue) from 0.1.0.post0 to 0.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dbluhm/async-selective-queue/releases">async-selective-queue's releases</a>.</em></p>
<blockquote>
<h2>v0.1.1</h2>
<p>This release comes with the following major changes:</p>
<ul>
<li>Python 3.7 and 3.8 support has been dropped</li>
<li>Poetry has been dropped in favor of PDM</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>refactor: rework project by <a href="https://github.com/dbluhm"><code>@​dbluhm</code></a> in <a href="https://redirect.github.com/dbluhm/async-selective-queue/pull/3">dbluhm/async-selective-queue#3</a></li>
<li>chore(deps): Bump the all-actions group with 2 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/dbluhm/async-selective-queue/pull/4">dbluhm/async-selective-queue#4</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/dependabot"><code>@​dependabot</code></a> made their first contribution in <a href="https://redirect.github.com/dbluhm/async-selective-queue/pull/4">dbluhm/async-selective-queue#4</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/dbluhm/async-selective-queue/compare/v0.1.0...v0.1.1">https://github.com/dbluhm/async-selective-queue/compare/v0.1.0...v0.1.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/dbluhm/async-selective-queue/commits/v0.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async-selective-queue&package-manager=pip&previous-version=0.1.0.post0&new-version=0.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/506" class=".btn">#506</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-alpine to 3.12-alpine in /kafka_events/demo/setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-alpine to 3.12-alpine.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-alpine&new-version=3.12-alpine)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/505" class=".btn">#505</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-slim to 3.12-slim in /basicmessage_storage/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-slim to 3.12-slim.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-slim&new-version=3.12-slim)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/504" class=".btn">#504</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.1 in /rpc/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/66ff8dffdf9eee9b3dd6686de34542c49ff80dcd"><code>66ff8df</code></a> Prepare release version 8.2.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3ffcfd122cf4674ac45f6233d9b50be6c49abeea"><code>3ffcfd1</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12340">#12340</a> from pytest-dev/backport-12334-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0b28313b46a04de08bddc18896b3e61312a0c5b3"><code>0b28313</code></a> [8.2.x] Add Python 3.13 (beta) support</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f3dd93ad8d62eb0a260d3090f31be82aafbcff13"><code>f3dd93a</code></a> [8.2.x] Attest package provenance (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12335">#12335</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bb5a1257b0aafe5932377fa8e9fd92ab39418ac7"><code>bb5a125</code></a> [8.2.x] Spelling (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12331">#12331</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f179bf252fe2c1d0afce64b4b4bab4449e366e84"><code>f179bf2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12327">#12327</a> from pytest-dev/backport-12325-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2b671b5f9208650e8e42e07782d95477cc41f42a"><code>2b671b5</code></a> [8.2.x] cacheprovider: fix <code>.pytest_cache</code> not being world-readable</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/65ab7cb96c95f83e922f21bb4a8a44eda2b79707"><code>65ab7cb</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12324">#12324</a> from pytest-dev/backport-12320-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4d5fb7d71ccc069e2f882bee0e4253eaf484d2a9"><code>4d5fb7d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12319">#12319</a> from pytest-dev/backport-12311-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/cbe5996cc684b00397494d9590f3179de232c3ee"><code>cbe5996</code></a> [8.2.x] changelog: document unittest 8.2 change as breaking</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/503" class=".btn">#503</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-slim-bookworm to 3.12-slim-bookworm in /oid4vci/integration/afj_runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-slim-bookworm to 3.12-slim-bookworm.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-slim-bookworm&new-version=3.12-slim-bookworm)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    Bump python from 3.9-slim to 3.12-slim in /connection_update/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.9-slim to 3.12-slim.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.9-slim&new-version=3.12-slim)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/501" class=".btn">#501</a>
            </td>
            <td>
                <b>
                    Bump python from 3.10-slim-bookworm to 3.12-slim-bookworm in /oid4vci/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.10-slim-bookworm to 3.12-slim-bookworm.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.10-slim-bookworm&new-version=3.12-slim-bookworm)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/500" class=".btn">#500</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.1 in /multitenant_provider/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/66ff8dffdf9eee9b3dd6686de34542c49ff80dcd"><code>66ff8df</code></a> Prepare release version 8.2.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3ffcfd122cf4674ac45f6233d9b50be6c49abeea"><code>3ffcfd1</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12340">#12340</a> from pytest-dev/backport-12334-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0b28313b46a04de08bddc18896b3e61312a0c5b3"><code>0b28313</code></a> [8.2.x] Add Python 3.13 (beta) support</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f3dd93ad8d62eb0a260d3090f31be82aafbcff13"><code>f3dd93a</code></a> [8.2.x] Attest package provenance (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12335">#12335</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bb5a1257b0aafe5932377fa8e9fd92ab39418ac7"><code>bb5a125</code></a> [8.2.x] Spelling (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12331">#12331</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f179bf252fe2c1d0afce64b4b4bab4449e366e84"><code>f179bf2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12327">#12327</a> from pytest-dev/backport-12325-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2b671b5f9208650e8e42e07782d95477cc41f42a"><code>2b671b5</code></a> [8.2.x] cacheprovider: fix <code>.pytest_cache</code> not being world-readable</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/65ab7cb96c95f83e922f21bb4a8a44eda2b79707"><code>65ab7cb</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12324">#12324</a> from pytest-dev/backport-12320-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4d5fb7d71ccc069e2f882bee0e4253eaf484d2a9"><code>4d5fb7d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12319">#12319</a> from pytest-dev/backport-12311-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/cbe5996cc684b00397494d9590f3179de232c3ee"><code>cbe5996</code></a> [8.2.x] changelog: document unittest 8.2 change as breaking</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/499" class=".btn">#499</a>
            </td>
            <td>
                <b>
                    Bump requests from 2.32.0 to 2.32.2 in /firebase_push_notifications/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.32.0 to 2.32.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.2</h2>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>v2.32.1</h2>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li><a href="https://github.com/psf/requests/commit/970e8cec988421bd43da57350723b05c8ce8dc7e"><code>970e8ce</code></a> v2.32.1</li>
<li>See full diff in <a href="https://github.com/psf/requests/compare/v2.32.0...v2.32.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.32.0&new-version=2.32.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    Bump requests from 2.32.0 to 2.32.2 in /basicmessage_storage/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.32.0 to 2.32.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.2</h2>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>v2.32.1</h2>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.2 (2024-05-21)</h2>
<p><strong>Deprecations</strong></p>
<ul>
<li>
<p>To provide a more stable migration for custom HTTPAdapters impacted
by the CVE changes in 2.32.0, we've renamed <code>_get_connection</code> to
a new public API, <code>get_connection_with_tls_context</code>. Existing custom
HTTPAdapters will need to migrate their code to use this new API.
<code>get_connection</code> is considered deprecated in all versions of Requests&gt;=2.32.0.</p>
<p>A minimal (2-line) example has been provided in the linked PR to ease
migration, but we strongly urge users to evaluate if their custom adapter
is subject to the same issue described in CVE-2024-35195. (<a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a>)</p>
</li>
</ul>
<h2>2.32.1 (2024-05-20)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Add missing test certs to the sdist distributed on PyPI.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/88dce9d854797c05d0ff296b70e0430535ef8aaf"><code>88dce9d</code></a> v2.32.2</li>
<li><a href="https://github.com/psf/requests/commit/c98e4d133ef29c46a9b68cd783087218a8075e05"><code>c98e4d1</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6710">#6710</a> from nateprewitt/api_rename</li>
<li><a href="https://github.com/psf/requests/commit/92075b330a30b9883f466a43d3f7566ab849f91b"><code>92075b3</code></a> Add deprecation warning</li>
<li><a href="https://github.com/psf/requests/commit/aa1461b68aa73e2f6ec0e78c8853b635c76fd099"><code>aa1461b</code></a> Move _get_connection to get_connection_with_tls_context</li>
<li><a href="https://github.com/psf/requests/commit/970e8cec988421bd43da57350723b05c8ce8dc7e"><code>970e8ce</code></a> v2.32.1</li>
<li>See full diff in <a href="https://github.com/psf/requests/compare/v2.32.0...v2.32.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.32.0&new-version=2.32.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/497" class=".btn">#497</a>
            </td>
            <td>
                <b>
                    Bump node from 18 to 22 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps node from 18 to 22.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node&package-manager=docker&previous-version=18&new-version=22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/496" class=".btn">#496</a>
            </td>
            <td>
                <b>
                    Bump axios from 1.6.0 to 1.7.2 in /oid4vci/demo/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 1.6.0 to 1.7.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v1.7.2</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>fetch:</strong> enhance fetch API detection; (<a href="https://redirect.github.com/axios/axios/issues/6413">#6413</a>) (<a href="https://github.com/axios/axios/commit/4f79aef81b7c4644328365bfc33acf0a9ef595bc">4f79aef</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+3/-3 ([#6413](https://github.com/axios/axios/issues/6413) )">Dmitriy Mozgovoy</a></li>
</ul>
<h2>Release v1.7.1</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>fetch:</strong> fixed ReferenceError issue when TextEncoder is not available in the environment; (<a href="https://redirect.github.com/axios/axios/issues/6410">#6410</a>) (<a href="https://github.com/axios/axios/commit/733f15fe5bd2d67e1fadaee82e7913b70d45dc5e">733f15f</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+14/-9 ([#6410](https://github.com/axios/axios/issues/6410) )">Dmitriy Mozgovoy</a></li>
</ul>
<h2>Release v1.7.0</h2>
<h2>Release notes:</h2>
<h3>Features</h3>
<ul>
<li><strong>adapter:</strong> add fetch adapter; (<a href="https://redirect.github.com/axios/axios/issues/6371">#6371</a>) (<a href="https://github.com/axios/axios/commit/a3ff99b59d8ec2ab5dd049e68c043617a4072e42">a3ff99b</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><strong>core/axios:</strong> handle un-writable error stack (<a href="https://redirect.github.com/axios/axios/issues/6362">#6362</a>) (<a href="https://github.com/axios/axios/commit/81e0455b7b57fbaf2be16a73ebe0e6591cc6d8f9">81e0455</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+1015/-127 ([#6371](https://github.com/axios/axios/issues/6371) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/jasonsaayman" title="+30/-14 ()">Jay</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/alexandre-abrioux" title="+56/-6 ([#6362](https://github.com/axios/axios/issues/6362) )">Alexandre ABRIOUX</a></li>
</ul>
<h2>Release v1.7.0-beta.2</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>fetch:</strong> capitalize HTTP method names; (<a href="https://redirect.github.com/axios/axios/issues/6395">#6395</a>) (<a href="https://github.com/axios/axios/commit/ad3174a3515c3c2573f4bcb94818d582826f3914">ad3174a</a>)</li>
<li><strong>fetch:</strong> fix &amp; optimize progress capturing for cases when the request data has a nullish value or zero data length (<a href="https://redirect.github.com/axios/axios/issues/6400">#6400</a>) (<a href="https://github.com/axios/axios/commit/95a3e8e346cfd6a5548e171f2341df3235d0e26b">95a3e8e</a>)</li>
<li><strong>fetch:</strong> fix headers getting from a stream response; (<a href="https://redirect.github.com/axios/axios/issues/6401">#6401</a>) (<a href="https://github.com/axios/axios/commit/870e0a76f60d0094774a6a63fa606eec52a381af">870e0a7</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+99/-46 ([#6405](https://github.com/axios/axios/issues/6405) [#6404](https://github.com/axios/axios/issues/6404) [#6401](https://github.com/axios/axios/issues/6401) [#6400](https://github.com/axios/axios/issues/6400) [#6395](https://github.com/axios/axios/issues/6395) )">Dmitriy Mozgovoy</a></li>
</ul>
<h2>Release v1.7.0-beta.1</h2>
<h2>Release notes:</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/axios/axios/compare/v1.7.1...v1.7.2">1.7.2</a> (2024-05-21)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>fetch:</strong> enhance fetch API detection; (<a href="https://redirect.github.com/axios/axios/issues/6413">#6413</a>) (<a href="https://github.com/axios/axios/commit/4f79aef81b7c4644328365bfc33acf0a9ef595bc">4f79aef</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+3/-3 ([#6413](https://github.com/axios/axios/issues/6413) )">Dmitriy Mozgovoy</a></li>
</ul>
<h2><a href="https://github.com/axios/axios/compare/v1.7.0...v1.7.1">1.7.1</a> (2024-05-20)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>fetch:</strong> fixed ReferenceError issue when TextEncoder is not available in the environment; (<a href="https://redirect.github.com/axios/axios/issues/6410">#6410</a>) (<a href="https://github.com/axios/axios/commit/733f15fe5bd2d67e1fadaee82e7913b70d45dc5e">733f15f</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+14/-9 ([#6410](https://github.com/axios/axios/issues/6410) )">Dmitriy Mozgovoy</a></li>
</ul>
<h1><a href="https://github.com/axios/axios/compare/v1.7.0-beta.2...v1.7.0">1.7.0</a> (2024-05-19)</h1>
<h3>Features</h3>
<ul>
<li><strong>adapter:</strong> add fetch adapter; (<a href="https://redirect.github.com/axios/axios/issues/6371">#6371</a>) (<a href="https://github.com/axios/axios/commit/a3ff99b59d8ec2ab5dd049e68c043617a4072e42">a3ff99b</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><strong>core/axios:</strong> handle un-writable error stack (<a href="https://redirect.github.com/axios/axios/issues/6362">#6362</a>) (<a href="https://github.com/axios/axios/commit/81e0455b7b57fbaf2be16a73ebe0e6591cc6d8f9">81e0455</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+1015/-127 ([#6371](https://github.com/axios/axios/issues/6371) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/jasonsaayman" title="+30/-14 ()">Jay</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/alexandre-abrioux" title="+56/-6 ([#6362](https://github.com/axios/axios/issues/6362) )">Alexandre ABRIOUX</a></li>
</ul>
<h1><a href="https://github.com/axios/axios/compare/v1.7.0-beta.1...v1.7.0-beta.2">1.7.0-beta.2</a> (2024-05-19)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>fetch:</strong> capitalize HTTP method names; (<a href="https://redirect.github.com/axios/axios/issues/6395">#6395</a>) (<a href="https://github.com/axios/axios/commit/ad3174a3515c3c2573f4bcb94818d582826f3914">ad3174a</a>)</li>
<li><strong>fetch:</strong> fix &amp; optimize progress capturing for cases when the request data has a nullish value or zero data length (<a href="https://redirect.github.com/axios/axios/issues/6400">#6400</a>) (<a href="https://github.com/axios/axios/commit/95a3e8e346cfd6a5548e171f2341df3235d0e26b">95a3e8e</a>)</li>
<li><strong>fetch:</strong> fix headers getting from a stream response; (<a href="https://redirect.github.com/axios/axios/issues/6401">#6401</a>) (<a href="https://github.com/axios/axios/commit/870e0a76f60d0094774a6a63fa606eec52a381af">870e0a7</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/0e4f9fa29077ebee4499facea6be1492b42e8a26"><code>0e4f9fa</code></a> chore(release): v1.7.2 (<a href="https://redirect.github.com/axios/axios/issues/6414">#6414</a>)</li>
<li><a href="https://github.com/axios/axios/commit/4f79aef81b7c4644328365bfc33acf0a9ef595bc"><code>4f79aef</code></a> fix(fetch): enhance fetch API detection; (<a href="https://redirect.github.com/axios/axios/issues/6413">#6413</a>)</li>
<li><a href="https://github.com/axios/axios/commit/67d1373131962d1f1f5b8d91f9a2f80ed3923bc8"><code>67d1373</code></a> chore(release): v1.7.1 (<a href="https://redirect.github.com/axios/axios/issues/6411">#6411</a>)</li>
<li><a href="https://github.com/axios/axios/commit/733f15fe5bd2d67e1fadaee82e7913b70d45dc5e"><code>733f15f</code></a> fix(fetch): fixed ReferenceError issue when TextEncoder is not available in t...</li>
<li><a href="https://github.com/axios/axios/commit/3041c61adaaac6d2c43eba28c134e7f4d43ab012"><code>3041c61</code></a> [Release] v1.7.0 (<a href="https://redirect.github.com/axios/axios/issues/6408">#6408</a>)</li>
<li><a href="https://github.com/axios/axios/commit/18b13cbaef66d8c266cf681165afe31787420100"><code>18b13cb</code></a> chore(docs): add fetch adapter docs; (<a href="https://redirect.github.com/axios/axios/issues/6407">#6407</a>)</li>
<li><a href="https://github.com/axios/axios/commit/e62099bc8b640acf47fba639366bbcd3bf87f831"><code>e62099b</code></a> fix(fetch): fixed a possible memory leak in the AbortController for the strea...</li>
<li><a href="https://github.com/axios/axios/commit/b49aa8e3d837c36e4728a9fa8a5e23a1162e96ec"><code>b49aa8e</code></a> chore(release): v1.7.0-beta.2 (<a href="https://redirect.github.com/axios/axios/issues/6403">#6403</a>)</li>
<li><a href="https://github.com/axios/axios/commit/d57f03a77fef1eb3cd9a17e2973c4305e105a42e"><code>d57f03a</code></a> chore(ci): bump create-pull-request version to fix a bug; (<a href="https://redirect.github.com/axios/axios/issues/6405">#6405</a>)</li>
<li><a href="https://github.com/axios/axios/commit/097b0d18e93d12c53b77741d6bfdc8a1fc11828b"><code>097b0d1</code></a> chore(ci): add tag resolution for npm releases based on package version; (<a href="https://redirect.github.com/axios/axios/issues/6404">#6404</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v1.6.0...v1.7.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=1.6.0&new-version=1.7.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-22 16:17:14 +0000 UTC
    </div>
</div>

