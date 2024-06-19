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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/839" class=".btn">#839</a>
            </td>
            <td>
                <b>
                    Change parallelism to 1 in GHA runs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Attempts to address #835 .  We don’t really care how long the runs take, but we would like the results to be accurate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 05:35:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    Bump prettier from 2.8.8 to 3.3.2 in /aries-backchannels/javascript/server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [prettier](https://github.com/prettier/prettier) from 2.8.8 to 3.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/releases">prettier's releases</a>.</em></p>
<blockquote>
<h2>3.3.2</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#332">Changelog</a></p>
<h2>3.3.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#331">Changelog</a></p>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md">prettier's changelog</a>.</em></p>
<blockquote>
<h1>3.3.2</h1>
<p><a href="https://github.com/prettier/prettier/compare/3.3.1...3.3.2">diff</a></p>
<h4>Fix handlebars path expressions starts with <code>@</code> (<a href="https://redirect.github.com/prettier/prettier/pull/16358">#16358</a> by <a href="https://github.com/Princeyadav05"><code>@​Princeyadav05</code></a>)</h4>
<!-- raw HTML omitted -->
<pre lang="hbs"><code>{{! Input }}
&lt;div&gt;{{@x.y.z}}&lt;/div&gt;
<p>{{! Prettier 3.3.1 }}
&lt;div&gt;{{<a href="https://github.com/x"><code>@​x</code></a>}}&lt;/div&gt;</p>
<p>{{! Prettier 3.3.2 }}
&lt;div&gt;{{<a href="https://github.com/x"><code>@​x</code></a>.y.z}}&lt;/div&gt;
</code></pre></p>
<h1>3.3.1</h1>
<p><a href="https://github.com/prettier/prettier/compare/3.3.0...3.3.1">diff</a></p>
<h4>Preserve empty lines in front matter (<a href="https://redirect.github.com/prettier/prettier/pull/16347">#16347</a> by <a href="https://github.com/fisker"><code>@​fisker</code></a>)</h4>
<!-- raw HTML omitted -->
<pre lang="markdown"><code>&lt;!-- Input --&gt;
---
foo:
  - bar1
<ul>
<li>
<p>bar2</p>
</li>
<li>
<p>bar3</p>
</li>
</ul>
<hr />
<p>Markdown</p>
<p>&lt;!-- Prettier 3.3.0 --&gt;</p>
<hr />
<p>foo:</p>
<ul>
<li>bar1</li>
<li>bar2</li>
<li>bar3</li>
</ul>
<hr />
<p>Markdown</p>
<p>&lt;!-- Prettier 3.3.1 --&gt;
&lt;/tr&gt;&lt;/table&gt;
</code></pre></p>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prettier/prettier/commit/1596a608dedac55c20bad3f1b5bfd47f961c696b"><code>1596a60</code></a> Release 3.3.2</li>
<li><a href="https://github.com/prettier/prettier/commit/aebcee5ea49ff0ee934ce39d26edb09cbd3f17db"><code>aebcee5</code></a> chore(deps): update dependency esbuild to v0.21.5 (<a href="https://redirect.github.com/prettier/prettier/issues/16379">#16379</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/57aa9287a078f0ed266e779bd00528fff2598bb2"><code>57aa928</code></a> chore(deps): update dependency c8 to v10 (<a href="https://redirect.github.com/prettier/prettier/issues/16380">#16380</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/c3d0b7f419f6f51876bbb1fc36b9755b8c9dcb8e"><code>c3d0b7f</code></a> chore(deps): update typescript-eslint to v7.13.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16376">#16376</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/27c35db5e20a121aad0cc3fff7a80658b7503ea0"><code>27c35db</code></a> chore(deps): update dependency codemirror-graphql to v2.0.12 (<a href="https://redirect.github.com/prettier/prettier/issues/16369">#16369</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/6de325866695e23269d0d217cf73c4cc0340226e"><code>6de3258</code></a> chore(deps): update dependency jest to v30.0.0-alpha.5 (<a href="https://redirect.github.com/prettier/prettier/issues/16371">#16371</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/b5f983d2bb24ae78ba560c7d57c4b1753ea32cfa"><code>b5f983d</code></a> Upgrade yarn to v4.3.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16377">#16377</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/d6f37c4109e97fdfa054d7af147e82495a18d1c7"><code>d6f37c4</code></a> chore(deps): update dependency browserslist to v4.23.1 (<a href="https://redirect.github.com/prettier/prettier/issues/16368">#16368</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/5055b7d39265fddae29917390c83ef28df497f23"><code>5055b7d</code></a> chore(deps): update dependency execa to v9.2.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16372">#16372</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/f4608cc76b097a03487f00132a904dea1312c56d"><code>f4608cc</code></a> chore(deps): update dependency cspell to v8.8.4 (<a href="https://redirect.github.com/prettier/prettier/issues/16370">#16370</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/prettier/prettier/compare/2.8.8...3.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=prettier&package-manager=npm_and_yarn&previous-version=2.8.8&new-version=3.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-17 11:16:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/837" class=".btn">#837</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 02:27:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/836" class=".btn">#836</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-16 19:32:44 +0000 UTC
    </div>
</div>

