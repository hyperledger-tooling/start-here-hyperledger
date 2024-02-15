---
layout: default
title: indy-did-method
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-did-method
---

# indy-did-method <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-did-method){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Bump markdown-it and spec-up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                [//]: # (dependabot-start)
⚠️  **Dependabot is rebasing this PR** ⚠️ 

Rebasing might not happen immediately, so don't worry if this takes some time.

Note: if you make any changes to this PR yourself, they will take precedence over the rebase.

---

[//]: # (dependabot-end)

Bumps [markdown-it](https://github.com/markdown-it/markdown-it) to 13.0.1 and updates ancestor dependency [spec-up](https://github.com/decentralized-identity/spec-up). These dependencies need to be updated together.

Updates `markdown-it` from 8.4.2 to 13.0.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/markdown-it/markdown-it/blob/master/CHANGELOG.md">markdown-it's changelog</a>.</em></p>
<blockquote>
<h2>[13.0.1] - 2022-05-03</h2>
<h3>Fixed</h3>
<ul>
<li>Bumped <code>linkify-it</code> to 4.0.1. That should fix some hangs, caused by wrong
data, returned from <code>linkify-it</code>.</li>
</ul>
<h2>[13.0.0] - 2022-04-22</h2>
<h3>Added</h3>
<ul>
<li>Added a new token type <code>text_special</code> to store escaped characters, same as <code>text</code> but
unaffected by replacement plugins (smartquotes, typographer, linkifier, etc.).</li>
<li>Added a new rule <code>text_join</code> in <code>core</code> ruler. Text replacement plugins may choose to
insert themselves before it.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>(p)</code> is no longer replaced with § by typographer (conflicts with ℗), <a href="https://redirect.github.com/markdown-it/markdown-it/issues/763">#763</a>.</li>
<li><code>text_collapse</code> rule is renamed to <code>fragments_join</code>.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Smartquotes, typographic replacements and plain text links can now be escaped
with backslash (e.g. <code>\(c)</code> or <code>google\.com</code> are no longer replaced).</li>
<li>Fixed collision of emphasis and linkifier (so <code>http://example.org/foo._bar_-_baz</code>
is now a single link, not emphasized). Emails and fuzzy links are not affected by this.</li>
</ul>
<h2>[12.3.2] - 2022-01-08</h2>
<h3>Security</h3>
<ul>
<li>Fix possible ReDOS in newline rule. Thanks to <a href="https://github.com/MakeNowJust"><code>@​MakeNowJust</code></a>.</li>
</ul>
<h2>[12.3.1] - 2022-01-07</h2>
<h3>Fixed</h3>
<ul>
<li>Fix corner case when tab prevents paragraph continuation in lists, <a href="https://redirect.github.com/markdown-it/markdown-it/issues/830">#830</a>.</li>
</ul>
<h2>[12.3.0] - 2021-12-09</h2>
<h3>Changed</h3>
<ul>
<li><code>StateInline.delimiters[].jump</code> is removed.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fixed quadratic complexity in pathological <code>***&lt;10k stars&gt;***a***&lt;10k stars&gt;***</code> case.</li>
</ul>
<h2>[12.2.0] - 2021-08-02</h2>
<h3>Added</h3>
<ul>
<li>Ordered lists: add order value to token info.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Always suffix indented code block with a newline, <a href="https://redirect.github.com/markdown-it/markdown-it/issues/799">#799</a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/markdown-it/markdown-it/commit/e843acc9edad115cbf8cf85e676443f01658be08"><code>e843acc</code></a> Merge branch 'master' of github.com:markdown-it/markdown-it</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/bda718216b20fa03b725443b8a1d160a0baeb94f"><code>bda7182</code></a> 13.0.1 released</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/b8b610fd7ae2783cee110539b5429d9b09671409"><code>b8b610f</code></a> Dist rebuild</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/d17df137d08e0cf989c21223dfbb420fac929a51"><code>d17df13</code></a> Bump linkify-it to 4.0.1</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/0c19c372231ad71bb788345071d7c48c9f7fbf35"><code>0c19c37</code></a> Merge pull request <a href="https://redirect.github.com/markdown-it/markdown-it/issues/866">#866</a> from yne/patch-1</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/e157cd242bbed14857a59d533091515ed905f189"><code>e157cd2</code></a> doc: Add syntax highlighting</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/6ec0b76ebe439f5858ae51d8e0cb45ee4a7ad46c"><code>6ec0b76</code></a> 13.0.0 released</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/0e4c0f47a9ef87c07016a1f39b817dd3585eb19b"><code>0e4c0f4</code></a> Dist rebuild</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/d1757ed98b57d17b2656c6abe314efdccabc9732"><code>d1757ed</code></a> Bump linkify-it to v4</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/bab0baf193d78d974ceb22c45bf05fff1741db08"><code>bab0baf</code></a> Added examples on how to add and modify rules (<a href="https://redirect.github.com/markdown-it/markdown-it/issues/619">#619</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/markdown-it/markdown-it/compare/8.4.2...13.0.1">compare view</a></li>
</ul>
</details>
<br />

Updates `spec-up` from 0.10.1 to 0.10.6
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/decentralized-identity/spec-up/commits">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-did-method/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 18:27:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Bump prismjs and spec-up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [prismjs](https://github.com/PrismJS/prism) to 1.29.0 and updates ancestor dependency [spec-up](https://github.com/decentralized-identity/spec-up). These dependencies need to be updated together.

Updates `prismjs` from 1.21.0 to 1.29.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/PrismJS/prism/releases">prismjs's releases</a>.</em></p>
<blockquote>
<h2>v1.29.0</h2>
<p>Release 1.29.0</p>
<h2>v1.28.0</h2>
<p>Release 1.28.0</p>
<h2>v1.27.0</h2>
<p>Release 1.27.0</p>
<h2>v1.26.0</h2>
<p>Release 1.26.0</p>
<h2>v1.25.0</h2>
<p>Release 1.25.0</p>
<h2>v1.24.1</h2>
<p>Release 1.24.1</p>
<h2>v1.24.0</h2>
<p>Release 1.24.0</p>
<h2>v1.23.0</h2>
<p>Release 1.23.0</p>
<h2>v1.22.0</h2>
<p>Release 1.22.0</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/PrismJS/prism/blob/master/CHANGELOG.md">prismjs's changelog</a>.</em></p>
<blockquote>
<h2>1.29.0 (2022-08-23)</h2>
<h3>New components</h3>
<ul>
<li><strong>BBj</strong> (<a href="https://redirect.github.com/PrismJS/prism/issues/3511">#3511</a>) <a href="https://github.com/PrismJS/prism/commit/1134bdfc"><code>1134bdfc</code></a></li>
<li><strong>BQN</strong> (<a href="https://redirect.github.com/PrismJS/prism/issues/3515">#3515</a>) <a href="https://github.com/PrismJS/prism/commit/859f99a0"><code>859f99a0</code></a></li>
<li><strong>Cilk/C</strong> &amp; <strong>Cilk/C++</strong> (<a href="https://redirect.github.com/PrismJS/prism/issues/3522">#3522</a>) <a href="https://github.com/PrismJS/prism/commit/c8462a29"><code>c8462a29</code></a></li>
<li><strong>Gradle</strong> (<a href="https://redirect.github.com/PrismJS/prism/issues/3443">#3443</a>) <a href="https://github.com/PrismJS/prism/commit/32119823"><code>32119823</code></a></li>
<li><strong>METAFONT</strong> (<a href="https://redirect.github.com/PrismJS/prism/issues/3465">#3465</a>) <a href="https://github.com/PrismJS/prism/commit/2815f699"><code>2815f699</code></a></li>
<li><strong>WGSL</strong> (<a href="https://redirect.github.com/PrismJS/prism/issues/3455">#3455</a>) <a href="https://github.com/PrismJS/prism/commit/4c87d418"><code>4c87d418</code></a></li>
</ul>
<h3>Updated components</h3>
<ul>
<li><strong>AsciiDoc</strong>
<ul>
<li>Some regexes are too greedy (<a href="https://redirect.github.com/PrismJS/prism/issues/3481">#3481</a>) <a href="https://github.com/PrismJS/prism/commit/c4cbeeaa"><code>c4cbeeaa</code></a></li>
</ul>
</li>
<li><strong>Bash</strong>
<ul>
<li>Added &quot;sh&quot; alias (<a href="https://redirect.github.com/PrismJS/prism/issues/3509">#3509</a>) <a href="https://github.com/PrismJS/prism/commit/6b824d47"><code>6b824d47</code></a></li>
<li>Added support for parameters and the <code>java</code> and <code>sysctl</code> commands. (<a href="https://redirect.github.com/PrismJS/prism/issues/3505">#3505</a>) <a href="https://github.com/PrismJS/prism/commit/b9512b22"><code>b9512b22</code></a></li>
<li>Added <code>cargo</code> command (<a href="https://redirect.github.com/PrismJS/prism/issues/3488">#3488</a>) <a href="https://github.com/PrismJS/prism/commit/3e937137"><code>3e937137</code></a></li>
</ul>
</li>
<li><strong>BBj</strong>
<ul>
<li>Improve regexes (<a href="https://redirect.github.com/PrismJS/prism/issues/3512">#3512</a>) <a href="https://github.com/PrismJS/prism/commit/0cad9ae5"><code>0cad9ae5</code></a></li>
</ul>
</li>
<li><strong>CSS</strong>
<ul>
<li>Fixed @-rules not accounting for strings (<a href="https://redirect.github.com/PrismJS/prism/issues/3438">#3438</a>) <a href="https://github.com/PrismJS/prism/commit/0d4b6cb6"><code>0d4b6cb6</code></a></li>
</ul>
</li>
<li><strong>CSS Extras</strong>
<ul>
<li>Added support for <code>RebeccaPurple</code> color (<a href="https://redirect.github.com/PrismJS/prism/issues/3448">#3448</a>) <a href="https://github.com/PrismJS/prism/commit/646b2e0a"><code>646b2e0a</code></a></li>
</ul>
</li>
<li><strong>Hoon</strong>
<ul>
<li>Fixed escaped strings (<a href="https://redirect.github.com/PrismJS/prism/issues/3473">#3473</a>) <a href="https://github.com/PrismJS/prism/commit/64642716"><code>64642716</code></a></li>
</ul>
</li>
<li><strong>Java</strong>
<ul>
<li>Added support for constants (<a href="https://redirect.github.com/PrismJS/prism/issues/3507">#3507</a>) <a href="https://github.com/PrismJS/prism/commit/342a0039"><code>342a0039</code></a></li>
</ul>
</li>
<li><strong>Markup</strong>
<ul>
<li>Fixed quotes in HTML attribute values (<a href="https://redirect.github.com/PrismJS/prism/issues/3442">#3442</a>) <a href="https://github.com/PrismJS/prism/commit/ca8eaeee"><code>ca8eaeee</code></a></li>
</ul>
</li>
<li><strong>NSIS</strong>
<ul>
<li>Added missing commands (<a href="https://redirect.github.com/PrismJS/prism/issues/3504">#3504</a>) <a href="https://github.com/PrismJS/prism/commit/b0c2a9b4"><code>b0c2a9b4</code></a></li>
</ul>
</li>
<li><strong>Scala</strong>
<ul>
<li>Updated keywords to support Scala 3 (<a href="https://redirect.github.com/PrismJS/prism/issues/3506">#3506</a>) <a href="https://github.com/PrismJS/prism/commit/a090d063"><code>a090d063</code></a></li>
</ul>
</li>
<li><strong>SCSS</strong>
<ul>
<li>Fix casing in title of the <code>scss</code> lang (<a href="https://redirect.github.com/PrismJS/prism/issues/3501">#3501</a>) <a href="https://github.com/PrismJS/prism/commit/2aed9ce7"><code>2aed9ce7</code></a></li>
</ul>
</li>
</ul>
<h3>Updated plugins</h3>
<ul>
<li><strong>Line Highlight</strong>
<ul>
<li>Account for offset when clamping ranges (<a href="https://redirect.github.com/PrismJS/prism/issues/3518">#3518</a>) <a href="https://github.com/PrismJS/prism/commit/098e3000"><code>098e3000</code></a></li>
<li>Ignore ranges outside of actual lines (<a href="https://redirect.github.com/PrismJS/prism/issues/3475">#3475</a>) <a href="https://github.com/PrismJS/prism/commit/9a4e725b"><code>9a4e725b</code></a></li>
</ul>
</li>
<li><strong>Normalize Whitespace</strong>
<ul>
<li>Add configuration via attributes (<a href="https://redirect.github.com/PrismJS/prism/issues/3467">#3467</a>) <a href="https://github.com/PrismJS/prism/commit/91dea0c8"><code>91dea0c8</code></a></li>
</ul>
</li>
</ul>
<h3>Other</h3>
<ul>
<li>Added security policy (<a href="https://redirect.github.com/PrismJS/prism/issues/3070">#3070</a>) <a href="https://github.com/PrismJS/prism/commit/05ee042a"><code>05ee042a</code></a></li>
<li>Added list of maintainers (<a href="https://redirect.github.com/PrismJS/prism/issues/3410">#3410</a>) <a href="https://github.com/PrismJS/prism/commit/866b302e"><code>866b302e</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/PrismJS/prism/commit/59e5a3471377057de1f401ba38337aca27b80e03"><code>59e5a34</code></a> 1.29.0</li>
<li><a href="https://github.com/PrismJS/prism/commit/cd080f25ba12ef792d11468f5633fbbb23fd390e"><code>cd080f2</code></a> Updated npmignore to include new MD files (<a href="https://redirect.github.com/PrismJS/prism/issues/3534">#3534</a>)</li>
<li><a href="https://github.com/PrismJS/prism/commit/751664bd300b16b7b715e544de5a164b91b03075"><code>751664b</code></a> Added PR stop notice (<a href="https://redirect.github.com/PrismJS/prism/issues/3532">#3532</a>)</li>
<li><a href="https://github.com/PrismJS/prism/commit/248f6abb7074ff1dc48d289ea52ce99bd43eccb1"><code>248f6ab</code></a> Added changelog for v1.29.0 (<a href="https://redirect.github.com/PrismJS/prism/issues/3533">#3533</a>)</li>
<li><a href="https://github.com/PrismJS/prism/commit/098e30008eefc45874f5a32b4ce7141534060890"><code>098e300</code></a> Line Highlight: Account for offset when clamping ranges (<a href="https://redirect.github.com/PrismJS/prism/issues/3518">#3518</a>)</li>
<li><a href="https://github.com/PrismJS/prism/commit/6b824d479f26e4c922640604e14245f2cef52bb3"><code>6b824d4</code></a> Bash: Added &quot;sh&quot; alias (<a href="https://redirect.github.com/PrismJS/prism/issues/3509">#3509</a>)</li>
<li><a href="https://github.com/PrismJS/prism/commit/15272f76ff3b7aaa1bfe40decff0844b575eb5e5"><code>15272f7</code></a> Website: Added third-party tutorial for Pug template (<a href="https://redirect.github.com/PrismJS/prism/issues/3459">#3459</a>)</li>
<li><a href="https://github.com/PrismJS/prism/commit/c8462a29fb2853a5309b0532998a6198f08c4ca3"><code>c8462a2</code></a> Cilk: Add support for Cilk (with C/C++) (<a href="https://redirect.github.com/PrismJS/prism/issues/3522">#3522</a>)</li>
<li><a href="https://github.com/PrismJS/prism/commit/859f99a042e2f9c072a882b4cf9bf5f1f7804fa9"><code>859f99a</code></a> Added bqn language support (<a href="https://redirect.github.com/PrismJS/prism/issues/3515">#3515</a>)</li>
<li><a href="https://github.com/PrismJS/prism/commit/0cad9ae52d81095ecd34a3d17ac1e2526f1b48cd"><code>0cad9ae</code></a> BBj: Improve regexes (<a href="https://redirect.github.com/PrismJS/prism/issues/3512">#3512</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/PrismJS/prism/compare/v1.21.0...v1.29.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~rundevelopment">rundevelopment</a>, a new releaser for prismjs since your current version.</p>
</details>
<br />

Updates `spec-up` from 0.10.1 to 0.10.6
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/decentralized-identity/spec-up/commits">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-did-method/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 18:27:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Bump semver from 5.7.1 to 5.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [semver](https://github.com/npm/node-semver) from 5.7.1 to 5.7.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v5.7.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v5.7.1...v5.7.2">5.7.2</a> (2023-07-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/2f8fd41487acf380194579ecb6f8b1bbfe116be0"><code>2f8fd41</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/585">#585</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/585">#585</a>) (<a href="https://github.com/joaomoreno"><code>@​joaomoreno</code></a>, <a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/v5.7.2/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v5.7.1...v5.7.2">5.7.2</a> (2023-07-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/2f8fd41487acf380194579ecb6f8b1bbfe116be0"><code>2f8fd41</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/585">#585</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/585">#585</a>) (<a href="https://github.com/joaomoreno"><code>@​joaomoreno</code></a>, <a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>5.7</h2>
<ul>
<li>Add <code>minVersion</code> method</li>
</ul>
<h2>5.6</h2>
<ul>
<li>Move boolean <code>loose</code> param to an options object, with
backwards-compatibility protection.</li>
<li>Add ability to opt out of special prerelease version handling with
the <code>includePrerelease</code> option flag.</li>
</ul>
<h2>5.5</h2>
<ul>
<li>Add version coercion capabilities</li>
</ul>
<h2>5.4</h2>
<ul>
<li>Add intersection checking</li>
</ul>
<h2>5.3</h2>
<ul>
<li>Add <code>minSatisfying</code> method</li>
</ul>
<h2>5.2</h2>
<ul>
<li>Add <code>prerelease(v)</code> that returns prerelease components</li>
</ul>
<h2>5.1</h2>
<ul>
<li>Add Backus-Naur for ranges</li>
<li>Remove excessively cute inspection methods</li>
</ul>
<h2>5.0</h2>
<ul>
<li>Remove AMD/Browserified build artifacts</li>
<li>Fix ltr and gtr when using the <code>*</code> range</li>
<li>Fix for range <code>*</code> with a prerelease identifier</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/f8cc313550691a50d9662d8c94f0c033717efd7d"><code>f8cc313</code></a> chore: release 5.7.2</li>
<li><a href="https://github.com/npm/node-semver/commit/2f8fd41487acf380194579ecb6f8b1bbfe116be0"><code>2f8fd41</code></a> fix: better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/585">#585</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/deb5ad51bf58868fa243c1683775305fe9e0e365"><code>deb5ad5</code></a> chore: <code>@​npmcli/template-oss</code><a href="https://github.com/4"><code>@​4</code></a>.16.0</li>
<li>See full diff in <a href="https://github.com/npm/node-semver/compare/v5.7.1...v5.7.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~lukekarrys">lukekarrys</a>, a new releaser for semver since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=semver&package-manager=npm_and_yarn&previous-version=5.7.1&new-version=5.7.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-did-method/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 18:25:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Bump follow-redirects from 1.14.8 to 1.15.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                [//]: # (dependabot-start)
⚠️  **Dependabot is rebasing this PR** ⚠️ 

Rebasing might not happen immediately, so don't worry if this takes some time.

Note: if you make any changes to this PR yourself, they will take precedence over the rebase.

---

[//]: # (dependabot-end)

Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.8 to 1.15.5.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/b1677ce00110ee50dc5da576751d39b281fc4944"><code>b1677ce</code></a> Release version 1.15.5 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/d8914f7982403ea096b39bd594a00ee9d3b7e224"><code>d8914f7</code></a> Preserve fragment in responseUrl.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/65858205e59f1e23c9bf173348a7a7cbb8ac47f5"><code>6585820</code></a> Release version 1.15.4 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/7a6567e16dfa9ad18a70bfe91784c28653fbf19d"><code>7a6567e</code></a> Disallow bracketed hostnames.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/05629af696588b90d64e738bc2e809a97a5f92fc"><code>05629af</code></a> Prefer native URL instead of deprecated url.parse.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/1cba8e85fa73f563a439fe460cf028688e4358df"><code>1cba8e8</code></a> Prefer native URL instead of legacy url.resolve.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/72bc2a4229bc18dc9fbd57c60579713e6264cb92"><code>72bc2a4</code></a> Simplify _processResponse error handling.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/3d42aecdca39b144a0a2f27ea134b4cf67dd796a"><code>3d42aec</code></a> Add bracket tests.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/bcbb096b32686ecad6cd34235358ed6f2217d4f0"><code>bcbb096</code></a> Do not directly set Error properties.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/192dbe7ce671ecad813c074bffe3b3f5d3680fee"><code>192dbe7</code></a> Release version 1.15.3 of the npm package.</li>
<li>Additional commits viewable in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.8...v1.15.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.8&new-version=1.15.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-did-method/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 18:25:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    Bump the all-actions group with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 2 updates: [actions/checkout](https://github.com/actions/checkout) and [JamesIves/github-pages-deploy-action](https://github.com/jamesives/github-pages-deploy-action).

Updates `actions/checkout` from 2 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/releases">actions/checkout's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update default runtime to node20 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li>Support fetching without the --progress option by <a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
<li>Release 4.0.0 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1447">actions/checkout#1447</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/takost"><code>@​takost</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li><a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v4.0.0">https://github.com/actions/checkout/compare/v3...v4.0.0</a></p>
<h2>v3.6.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Mark test scripts with Bash'isms to be run via Bash by <a href="https://github.com/dscho"><code>@​dscho</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1377">actions/checkout#1377</a></li>
<li>Add option to fetch tags even if fetch-depth &gt; 0 by <a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li>Release 3.6.0 by <a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li><a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.3...v3.6.0">https://github.com/actions/checkout/compare/v3.5.3...v3.6.0</a></p>
<h2>v3.5.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Checkout Issue in self hosted runner due to faulty submodule check-ins by <a href="https://github.com/megamanics"><code>@​megamanics</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li>Fix typos found by codespell by <a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li>Add support for sparse checkouts by <a href="https://github.com/dscho"><code>@​dscho</code></a> and <a href="https://github.com/dfdez"><code>@​dfdez</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
<li>Release v3.5.3 by <a href="https://github.com/TingluoHuang"><code>@​TingluoHuang</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1376">actions/checkout#1376</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/megamanics"><code>@​megamanics</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li><a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li><a href="https://github.com/dfdez"><code>@​dfdez</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v3.5.3">https://github.com/actions/checkout/compare/v3...v3.5.3</a></p>
<h2>v3.5.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Use correct API url / endpoint in GHES by <a href="https://github.com/fhammerl"><code>@​fhammerl</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1289">actions/checkout#1289</a> based on <a href="https://redirect.github.com/actions/checkout/issues/1286">#1286</a> by <a href="https://github.com/1newsr"><code>@​1newsr</code></a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.1...v3.5.2">https://github.com/actions/checkout/compare/v3.5.1...v3.5.2</a></p>
<h2>v3.5.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Improve checkout performance on Windows runners by upgrading <code>@​actions/github</code> dependency by <a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/blob/main/CHANGELOG.md">actions/checkout's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>v4.1.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1396">Add support for partial checkout filters</a></li>
</ul>
<h2>v4.0.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1067">Support fetching without the --progress option</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1436">Update to node20</a></li>
</ul>
<h2>v3.6.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1377">Fix: Mark test scripts with Bash'isms to be run via Bash</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/579">Add option to fetch tags even if fetch-depth &gt; 0</a></li>
</ul>
<h2>v3.5.3</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1196">Fix: Checkout fail in self-hosted runners when faulty submodule are checked-in</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1287">Fix typos found by codespell</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1369">Add support for sparse checkouts</a></li>
</ul>
<h2>v3.5.2</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1289">Fix api endpoint for GHES</a></li>
</ul>
<h2>v3.5.1</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1246">Fix slow checkout on Windows</a></li>
</ul>
<h2>v3.5.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1237">Add new public key for known_hosts</a></li>
</ul>
<h2>v3.4.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1209">Upgrade codeql actions to v2</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1210">Upgrade dependencies</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1225">Upgrade <code>@​actions/io</code></a></li>
</ul>
<h2>v3.3.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1045">Implement branch list using callbacks from exec function</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1050">Add in explicit reference to private checkout options</a></li>
<li>[Fix comment typos (that got added in <a href="https://redirect.github.com/actions/checkout/issues/770">#770</a>)](<a href="https://redirect.github.com/actions/checkout/pull/1057">actions/checkout#1057</a>)</li>
</ul>
<h2>v3.2.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/942">Add GitHub Action to perform release</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/967">Fix status badge</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1002">Replace datadog/squid with ubuntu/squid Docker image</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/964">Wrap pipeline commands for submoduleForeach in quotes</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1029">Update <code>@​actions/io</code> to 1.1.2</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1039">Upgrading version to 3.2.0</a></li>
</ul>
<h2>v3.1.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/939">Use <code>@​actions/core</code> <code>saveState</code> and <code>getState</code></a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/922">Add <code>github-server-url</code> input</a></li>
</ul>
<h2>v3.0.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/checkout/commit/b4ffde65f46336ab88eb53be808477a3936bae11"><code>b4ffde6</code></a> Link to release page from what's new section (<a href="https://redirect.github.com/actions/checkout/issues/1514">#1514</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8530928916aaef40f59e6f221989ccb31f5759e7"><code>8530928</code></a> Correct link to GitHub Docs (<a href="https://redirect.github.com/actions/checkout/issues/1511">#1511</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/7cdaf2fbc075e6f3b9ca94cfd6cec5adc8a75622"><code>7cdaf2f</code></a> Update CODEOWNERS to Launch team (<a href="https://redirect.github.com/actions/checkout/issues/1510">#1510</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8ade135a41bc03ea155e62e844d188df1ea18608"><code>8ade135</code></a> Prepare 4.1.0 release (<a href="https://redirect.github.com/actions/checkout/issues/1496">#1496</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/c533a0a4cfc4962971818edcfac47a2899e69799"><code>c533a0a</code></a> Add support for partial checkout filters (<a href="https://redirect.github.com/actions/checkout/issues/1396">#1396</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/72f2cec99f417b1a1c5e2e88945068983b7965f9"><code>72f2cec</code></a> Update README.md for V4 (<a href="https://redirect.github.com/actions/checkout/issues/1452">#1452</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/3df4ab11eba7bda6032a0b82a6bb43b11571feac"><code>3df4ab1</code></a> Release 4.0.0 (<a href="https://redirect.github.com/actions/checkout/issues/1447">#1447</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8b5e8b768746b50394015010d25e690bfab9dfbc"><code>8b5e8b7</code></a> Support fetching without the --progress option (<a href="https://redirect.github.com/actions/checkout/issues/1067">#1067</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/97a652b80035363df47baee5031ec8670b8878ac"><code>97a652b</code></a> Update default runtime to node20 (<a href="https://redirect.github.com/actions/checkout/issues/1436">#1436</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/f43a0e5ff2bd294095638e18286ca9a3d1956744"><code>f43a0e5</code></a> Release 3.6.0 (<a href="https://redirect.github.com/actions/checkout/issues/1437">#1437</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/checkout/compare/v2...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `JamesIves/github-pages-deploy-action` from 4.1.3 to 4.5.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jamesives/github-pages-deploy-action/releases">JamesIves/github-pages-deploy-action's releases</a>.</em></p>
<blockquote>
<h2>v4.5.0</h2>
<h2>What's Changed</h2>
<ul>
<li>The action is now built and run on Node 20.</li>
<li>Bump <code>@​types/node</code> from 20.4.1 to 20.4.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1399">JamesIves/github-pages-deploy-action#1399</a></li>
<li>Bump eslint-plugin-jest from 27.2.2 to 27.2.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1400">JamesIves/github-pages-deploy-action#1400</a></li>
<li>Bump word-wrap from 1.2.3 to 1.2.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1401">JamesIves/github-pages-deploy-action#1401</a></li>
<li>Bump eslint-config-prettier from 8.8.0 to 8.9.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1405">JamesIves/github-pages-deploy-action#1405</a></li>
<li>Bump <code>@​types/node</code> from 20.4.2 to 20.4.9 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1413">JamesIves/github-pages-deploy-action#1413</a></li>
<li>Bump eslint-config-prettier from 8.9.0 to 9.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1410">JamesIves/github-pages-deploy-action#1410</a></li>
<li>Upgrade Node for security by <a href="https://github.com/nickmccurdy"><code>@​nickmccurdy</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1437">JamesIves/github-pages-deploy-action#1437</a></li>
<li>doc: <code>.gitignore</code> matches not being deployed by <a href="https://github.com/sgasse"><code>@​sgasse</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1459">JamesIves/github-pages-deploy-action#1459</a></li>
<li>build(deps): bump actions/setup-node from 3 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1467">JamesIves/github-pages-deploy-action#1467</a></li>
<li>build(deps-dev): bump <code>@​types/node</code> from 20.4.9 to 20.9.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1474">JamesIves/github-pages-deploy-action#1474</a></li>
<li>Bump actions/checkout from 3 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1429">JamesIves/github-pages-deploy-action#1429</a></li>
<li>build(deps-dev): bump <code>@​types/node</code> from 20.9.0 to 20.10.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1479">JamesIves/github-pages-deploy-action#1479</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/sgasse"><code>@​sgasse</code></a> made their first contribution in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1459">JamesIves/github-pages-deploy-action#1459</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/JamesIves/github-pages-deploy-action/compare/v4.4.3...v4.5.0">https://github.com/JamesIves/github-pages-deploy-action/compare/v4.4.3...v4.5.0</a></p>
<h2>v4.4.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump <code>@​types/node</code> from 18.8.0 to 18.8.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1239">JamesIves/github-pages-deploy-action#1239</a></li>
<li>Bump webfactory/ssh-agent from 0.5.4 to 0.7.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1252">JamesIves/github-pages-deploy-action#1252</a></li>
<li>Bump <code>@​types/node</code> from 18.8.4 to 18.11.9 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1262">JamesIves/github-pages-deploy-action#1262</a></li>
<li>Bump eslint-plugin-jest from 27.0.4 to 27.1.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1268">JamesIves/github-pages-deploy-action#1268</a></li>
<li>Bump <code>@​types/node</code> from 18.11.9 to 18.11.10 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1276">JamesIves/github-pages-deploy-action#1276</a></li>
<li>Bump <code>@​types/node</code> from 18.11.10 to 18.11.13 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1283">JamesIves/github-pages-deploy-action#1283</a></li>
<li>Bump eslint-config-prettier from 8.5.0 to 8.6.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1293">JamesIves/github-pages-deploy-action#1293</a></li>
<li>Bump json5 from 2.1.1 to 2.2.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1294">JamesIves/github-pages-deploy-action#1294</a></li>
<li>Bump minimatch from 3.0.4 to 3.1.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1270">JamesIves/github-pages-deploy-action#1270</a></li>
<li>Bump decode-uri-component from 0.2.0 to 0.2.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1277">JamesIves/github-pages-deploy-action#1277</a></li>
<li>Bump typescript from 4.8.4 to 4.9.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1281">JamesIves/github-pages-deploy-action#1281</a></li>
<li>Bump eslint-plugin-jest from 27.1.5 to 27.2.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1296">JamesIves/github-pages-deploy-action#1296</a></li>
<li>Bump rimraf from 3.0.2 to 4.1.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1307">JamesIves/github-pages-deploy-action#1307</a></li>
<li>Bump typescript from 4.9.4 to 4.9.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1311">JamesIves/github-pages-deploy-action#1311</a></li>
<li>Bump codecov/codecov-action from 3.1.1 to 3.1.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1353">JamesIves/github-pages-deploy-action#1353</a></li>
<li>Bump <code>@​types/node</code> from 18.11.13 to 18.16.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1361">JamesIves/github-pages-deploy-action#1361</a></li>
<li>Bump codecov/codecov-action from 3.1.2 to 3.1.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1372">JamesIves/github-pages-deploy-action#1372</a></li>
<li>Bump <code>@​actions/io</code> from 1.1.2 to 1.1.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1339">JamesIves/github-pages-deploy-action#1339</a></li>
<li>Bump prettier from 2.7.1 to 2.8.8 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1357">JamesIves/github-pages-deploy-action#1357</a></li>
<li>Bump <code>@​types/node</code> from 18.16.3 to 20.2.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1380">JamesIves/github-pages-deploy-action#1380</a></li>
<li>Bump webfactory/ssh-agent from 0.7.0 to 0.8.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1348">JamesIves/github-pages-deploy-action#1348</a></li>
<li>Bump eslint-config-prettier from 8.6.0 to 8.8.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1342">JamesIves/github-pages-deploy-action#1342</a></li>
<li>Bump <code>@​types/node</code> from 20.2.3 to 20.2.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1381">JamesIves/github-pages-deploy-action#1381</a></li>
<li>Bump <code>@​types/node</code> from 20.2.4 to 20.2.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1383">JamesIves/github-pages-deploy-action#1383</a></li>
<li>Bump <code>@​types/node</code> from 20.2.5 to 20.3.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1385">JamesIves/github-pages-deploy-action#1385</a></li>
<li>Bump eslint-plugin-jest from 27.2.1 to 27.2.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1386">JamesIves/github-pages-deploy-action#1386</a></li>
<li>Bump <code>@​types/node</code> from 20.3.1 to 20.3.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/JamesIves/github-pages-deploy-action/pull/1387">JamesIves/github-pages-deploy-action#1387</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/65b5dfd4f5bcd3a7403bbc2959c144256167464e"><code>65b5dfd</code></a> Deploy Production Code for Commit 32bb2a8d7bda92f28b1fd223fc5793ab27f725eb 🚀</li>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/32bb2a8d7bda92f28b1fd223fc5793ab27f725eb"><code>32bb2a8</code></a> Merge branch 'dev' into releases/v4</li>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/7879c16b183e9e4d01df2ad341ca028096570343"><code>7879c16</code></a> feat: update to Node 20</li>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/1c34508fa25aca02eab9acba06e496d05744d1b4"><code>1c34508</code></a> build(deps-dev): bump <code>@​types/node</code> from 20.9.0 to 20.10.0 (<a href="https://redirect.github.com/jamesives/github-pages-deploy-action/issues/1479">#1479</a>)</li>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/b957d05c49f8a1699a3694a18f7f5ebafcd26f1b"><code>b957d05</code></a> Bump actions/checkout from 3 to 4 (<a href="https://redirect.github.com/jamesives/github-pages-deploy-action/issues/1429">#1429</a>)</li>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/3a4632deff2025662181e3731d352b4fffd4c5df"><code>3a4632d</code></a> build(deps-dev): bump <code>@​types/node</code> from 20.4.9 to 20.9.0 (<a href="https://redirect.github.com/jamesives/github-pages-deploy-action/issues/1474">#1474</a>)</li>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/9de026908021c3f454a557024a9c44136457ff4b"><code>9de0269</code></a> build(deps): bump actions/setup-node from 3 to 4 (<a href="https://redirect.github.com/jamesives/github-pages-deploy-action/issues/1467">#1467</a>)</li>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/810af534294f0668822498c26d1a0f3b11faa358"><code>810af53</code></a> Update README.md</li>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/24c1e2a9e444bcba7e87c995479bff311c3d1980"><code>24c1e2a</code></a> doc: <code>.gitignore</code> matches not being deployed (<a href="https://redirect.github.com/jamesives/github-pages-deploy-action/issues/1459">#1459</a>)</li>
<li><a href="https://github.com/JamesIves/github-pages-deploy-action/commit/0769273cc26fea2ee91b43a7f5110823f52df2c4"><code>0769273</code></a> fix: remove base.Dockerfile as it's not needed</li>
<li>Additional commits viewable in <a href="https://github.com/jamesives/github-pages-deploy-action/compare/4.1.3...v4.5.0">compare view</a></li>
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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 18:22:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Add Dependabot configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Configure Dependabot to automatically maintain dependencies for GitHub Actions.
  - Check for updates once a week.
  - Group all updates into a single PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 17:52:18 +0000 UTC
    </div>
</div>

