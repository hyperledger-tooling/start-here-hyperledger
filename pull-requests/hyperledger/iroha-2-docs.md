---
layout: default
title: iroha-2-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-2-docs
---

# iroha-2-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-2-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    Bump postcss from 8.4.27 to 8.4.31
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [postcss](https://github.com/postcss/postcss) from 8.4.27 to 8.4.31.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/releases">postcss's releases</a>.</em></p>
<blockquote>
<h2>8.4.31</h2>
<ul>
<li>Fixed <code>\r</code> parsing to fix CVE-2023-44270.</li>
</ul>
<h2>8.4.30</h2>
<ul>
<li>Improved source map performance (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>8.4.29</h2>
<ul>
<li>Fixed <code>Node#source.offset</code> (by <a href="https://github.com/idoros"><code>@​idoros</code></a>).</li>
<li>Fixed docs (by <a href="https://github.com/coliff"><code>@​coliff</code></a>).</li>
</ul>
<h2>8.4.28</h2>
<ul>
<li>Fixed <code>Root.source.end</code> for better source map (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed <code>Result.root</code> types when <code>process()</code> has no parser.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/blob/main/CHANGELOG.md">postcss's changelog</a>.</em></p>
<blockquote>
<h2>8.4.31</h2>
<ul>
<li>Fixed <code>\r</code> parsing to fix CVE-2023-44270.</li>
</ul>
<h2>8.4.30</h2>
<ul>
<li>Improved source map performance (by Romain Menke).</li>
</ul>
<h2>8.4.29</h2>
<ul>
<li>Fixed <code>Node#source.offset</code> (by Ido Rosenthal).</li>
<li>Fixed docs (by Christian Oliff).</li>
</ul>
<h2>8.4.28</h2>
<ul>
<li>Fixed <code>Root.source.end</code> for better source map (by Romain Menke).</li>
<li>Fixed <code>Result.root</code> types when <code>process()</code> has no parser.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/postcss/postcss/commit/90208de8805dd762596c0028b8637ffbed23e371"><code>90208de</code></a> Release 8.4.31 version</li>
<li><a href="https://github.com/postcss/postcss/commit/58cc860b4c1707510c9cd1bc1fa30b423a9ad6c5"><code>58cc860</code></a> Fix carrier return parsing</li>
<li><a href="https://github.com/postcss/postcss/commit/4fff8e4cdc237619df1d73a444c0a8329701c1e2"><code>4fff8e4</code></a> Improve pnpm test output</li>
<li><a href="https://github.com/postcss/postcss/commit/cd43ed123274a92ebc13a1e8cccf1d65b8198f84"><code>cd43ed1</code></a> Update dependencies</li>
<li><a href="https://github.com/postcss/postcss/commit/caa916bdcbf66c51321574e2dde112ab13e8b306"><code>caa916b</code></a> Update dependencies</li>
<li><a href="https://github.com/postcss/postcss/commit/8972f76923e921a3c9655822382039b31b1c8e1a"><code>8972f76</code></a> Typo</li>
<li><a href="https://github.com/postcss/postcss/commit/11a5286f781d2a637f2c545c5e9cd661055acaab"><code>11a5286</code></a> Typo</li>
<li><a href="https://github.com/postcss/postcss/commit/45c55017776fc61f7815d1ea8e92d5291ca5d6c8"><code>45c5501</code></a> Release 8.4.30 version</li>
<li><a href="https://github.com/postcss/postcss/commit/bc3c341f589f9c15f1b56838a33d908374e537e0"><code>bc3c341</code></a> Update linter</li>
<li><a href="https://github.com/postcss/postcss/commit/b2be58a2eb788d12474ee1335f8ecdb9fa6225aa"><code>b2be58a</code></a> Merge pull request <a href="https://redirect.github.com/postcss/postcss/issues/1881">#1881</a> from romainmenke/improve-sourcemap-performance--phil...</li>
<li>Additional commits viewable in <a href="https://github.com/postcss/postcss/compare/8.4.27...8.4.31">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=postcss&package-manager=npm_and_yarn&previous-version=8.4.27&new-version=8.4.31)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-2-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-08 01:16:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    Restructure docs, add home page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                what's new:
- added a home page with a nice layout
- split docs in 3 different parts as we discussed: get started, developer guide, api reference
- added navigation at the top (3 doc parts + troubleshooting)
- added an index page for get started section

<img width="813" alt="image" src="https://github.com/hyperledger/iroha-2-docs/assets/17865025/787c9e96-ffbc-467a-9d49-1bbce19584d2">

open questions:
- the naming of doc sections (get started, developer guide, api reference) -- if anyone has better ideas, please share
- one of the topics is not included in any table of contents: the `documenting/snippets` page is not a part of any doc part, idk if it even needs to be in our docs or not
- the docs don't follow SORA color theme, it's all default blue @0x009922 could you help with this? I think it'd be nice to have at least the home page with a custom SORA theme
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 22:37:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    [docs] #414: move API specification to the docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">iroha2</span>
            </td>
            <td>
                Closes #414

---

Source: https://github.com/hyperledger/iroha/blob/39b1ca1e6887a463d7f5fd8c45c83bb697ee8ea6/docs/source/references/api_spec.md

Changes:

- Fixed mentions of structures in requests/responses, linked them to the data-model page
- Changed structure & formatting of the document
- Put TODOs for future

If you have a better idea of how this page might look like, you are very welcome!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 07:37:04 +0000 UTC
    </div>
</div>

