---
layout: default
title: yui-docs
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-docs
---

# yui-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-docs/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Bump terser from 5.9.0 to 5.14.2 in /docsrcs/yui-ibc-solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 5.9.0 to 5.14.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v5.14.2</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
<li>Source maps improvements (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1211">#1211</a>)</li>
<li>Performance improvements in long property access evaluation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1213">#1213</a>)</li>
</ul>
<h2>v5.14.1</h2>
<ul>
<li>keep_numbers option added to TypeScript defs (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1208">#1208</a>)</li>
<li>Fixed parsing of nested template strings (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1204">#1204</a>)</li>
</ul>
<h2>v5.14.0</h2>
<ul>
<li>Switched to <code>@​jridgewell/source-map</code> for sourcemap generation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1190">#1190</a>, <a href="https://github-redirect.dependabot.com/terser/terser/issues/1181">#1181</a>)</li>
<li>Fixed source maps with non-terminated segments (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1106">#1106</a>)</li>
<li>Enabled typescript types to be imported from the package (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1194">#1194</a>)</li>
<li>Extra DOM props have been added (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1191">#1191</a>)</li>
<li>Delete the AST while generating code, as a means to save RAM</li>
</ul>
<h2>v5.13.1</h2>
<ul>
<li>Removed self-assignments (<code>varname=varname</code>) (closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1081">#1081</a>)</li>
<li>Separated inlining code (for inlining things into references, or removing IIFEs)</li>
<li>Allow multiple identifiers with the same name in <code>var</code> destructuring (eg <code>var { a, a } = x</code>) (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1176">#1176</a>)</li>
</ul>
<h2>v5.13.0</h2>
<ul>
<li>All calls to eval() were removed (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1171">#1171</a>, <a href="https://github-redirect.dependabot.com/terser/terser/issues/1184">#1184</a>)</li>
<li><code>source-map</code> was updated to 0.8.0-beta.0 (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1164">#1164</a>)</li>
<li>NavigatorUAData was added to domprops to avoid property mangling (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1166">#1166</a>)</li>
</ul>
<h2>v5.12.1</h2>
<ul>
<li>Fixed an issue with function definitions inside blocks (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1155">#1155</a>)</li>
<li>Fixed parens of <code>new</code> in some situations (closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1159">#1159</a>)</li>
</ul>
<h2>v5.12.0</h2>
<ul>
<li><code>TERSER_DEBUG_DIR</code> environment variable</li>
<li><a href="https://github.com/copyright"><code>@​copyright</code></a> comments are now preserved with the comments=&quot;some&quot; option (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1153">#1153</a>)</li>
</ul>
<h2>v5.11.0</h2>
<ul>
<li>Unicode code point escapes (<code>\u{abcde}</code>) are not emitted inside RegExp literals anymore (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1147">#1147</a>)</li>
<li>acorn is now a regular dependency</li>
</ul>
<h2>v5.10.0</h2>
<ul>
<li>Massive optimization to max_line_len (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1109">#1109</a>)</li>
<li>Basic support for import assertions</li>
<li>Marked ES2022 Object.hasOwn as a pure function</li>
<li>Fix <code>delete optional?.property</code></li>
<li>New CI/CD pipeline with github actions (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1057">#1057</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/terser/terser/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=5.9.0&new-version=5.14.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 19:09:26 +0000 UTC
    </div>
</div>

