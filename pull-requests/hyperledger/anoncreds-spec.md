---
layout: default
title: anoncreds-spec
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-spec
---

# anoncreds-spec <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-spec){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    Bump lodash.template and spec-up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [lodash.template](https://github.com/lodash/lodash). It's no longer used after updating ancestor dependency [spec-up](https://github.com/decentralized-identity/spec-up). These dependencies need to be updated together.

Removes `lodash.template`

Updates `spec-up` from 0.10.3 to 0.10.6
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/anoncreds-spec/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-03 17:04:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    Bump markdown-it and spec-up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
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
<li><code>(p)</code> is no longer replaced with § by typographer (conflicts with ℗), <a href="https://github-redirect.dependabot.com/markdown-it/markdown-it/issues/763">#763</a>.</li>
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
<li>Fix corner case when tab prevents paragraph continuation in lists, <a href="https://github-redirect.dependabot.com/markdown-it/markdown-it/issues/830">#830</a>.</li>
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
<li>Always suffix indented code block with a newline, <a href="https://github-redirect.dependabot.com/markdown-it/markdown-it/issues/799">#799</a>.</li>
</ul>
<h2>[12.1.0] - 2021-07-01</h2>
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
<li><a href="https://github.com/markdown-it/markdown-it/commit/0c19c372231ad71bb788345071d7c48c9f7fbf35"><code>0c19c37</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/markdown-it/markdown-it/issues/866">#866</a> from yne/patch-1</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/e157cd242bbed14857a59d533091515ed905f189"><code>e157cd2</code></a> doc: Add syntax highlighting</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/6ec0b76ebe439f5858ae51d8e0cb45ee4a7ad46c"><code>6ec0b76</code></a> 13.0.0 released</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/0e4c0f47a9ef87c07016a1f39b817dd3585eb19b"><code>0e4c0f4</code></a> Dist rebuild</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/d1757ed98b57d17b2656c6abe314efdccabc9732"><code>d1757ed</code></a> Bump linkify-it to v4</li>
<li><a href="https://github.com/markdown-it/markdown-it/commit/bab0baf193d78d974ceb22c45bf05fff1741db08"><code>bab0baf</code></a> Added examples on how to add and modify rules (<a href="https://github-redirect.dependabot.com/markdown-it/markdown-it/issues/619">#619</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/markdown-it/markdown-it/compare/8.4.2...13.0.1">compare view</a></li>
</ul>
</details>
<br />

Updates `spec-up` from 0.10.3 to 0.10.6
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/anoncreds-spec/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-03 17:03:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    Updates reflecting creation of Hyperledger AnonCreds and moving specification into the Hyperledger GitHub org
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-03 00:03:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Create maintainers file after transfer to Hyperledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-02 20:24:40 +0000 UTC
    </div>
</div>

