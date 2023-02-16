---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1271" class=".btn">#1271</a>
            </td>
            <td>
                <b>
                    Update minimum Java version.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Update the minimum Java version to Java 17+

## Issue fixed

Fixes #1270 

## Impacted parts

- [x] Documentation content
- [ ] Documentation page organization

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

- https://hyperledger-besu--1271.org.readthedocs.build/en/1271/public-networks/get-started/install/binary-distribution/
- https://hyperledger-besu--1271.org.readthedocs.build/en/1271/private-networks/get-started/install/binary-distribution/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 01:48:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    Bump markdown-include from 0.8.0 to 0.8.1 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [markdown-include](https://github.com/cmacmackin/markdown-include) from 0.8.0 to 0.8.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cmacmackin/markdown-include/releases">markdown-include's releases</a>.</em></p>
<blockquote>
<h2>v0.8.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix <code>inheritHeadingDepth</code> adding extra new lines by <a href="https://github.com/ldeluigi"><code>@​ldeluigi</code></a> in <a href="https://github-redirect.dependabot.com/cmacmackin/markdown-include/pull/43">cmacmackin/markdown-include#43</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/cmacmackin/markdown-include/compare/v0.8.0...v0.8.1">https://github.com/cmacmackin/markdown-include/compare/v0.8.0...v0.8.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/8da79f095c8ef7e37018387fac5b63b870de077b"><code>8da79f0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/cmacmackin/markdown-include/issues/43">#43</a> from cmacmackin/fix-inherit-heading-depth</li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/5135d01609e57b0052799fe5a67f2c2da6bfe060"><code>5135d01</code></a> Use more explicit <code>str.splitlines()</code></li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/7ae38cb8df9df7ed97e9169812675aa7a82a87d6"><code>7ae38cb</code></a> Fix <code>inheritHeadingDepth</code> adding extra newlines</li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/4e08bb867ca64f633c901b76d9773f2aceff0001"><code>4e08bb8</code></a> Remove sha-bang</li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/0ffd51029e55e9415454e16de968dc4026bc8f35"><code>0ffd510</code></a> Expand gitignore</li>
<li><a href="https://github.com/cmacmackin/markdown-include/commit/aa4a3800d71da83bfbe27ec80b62aa63ea652040"><code>aa4a380</code></a> Simplify test resource directory path</li>
<li>See full diff in <a href="https://github.com/cmacmackin/markdown-include/compare/v0.8.0...v0.8.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=markdown-include&package-manager=pip&previous-version=0.8.0&new-version=0.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 00:00:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1266" class=".btn">#1266</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 9.0.0 to 9.0.12 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.0.0 to 9.0.12.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.0.12</h2>
<ul>
<li>Updated Catalan translations</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4975">#4975</a>: Mermaid entity relationship rendering diagrams bug</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4924">#4924</a>: Header title not reset when using instant loading</li>
</ul>
<h2>mkdocs-material-9.0.11</h2>
<ul>
<li>Added Mastodon verification for social links (<code>rel=me</code>)</li>
<li>Updated Italian translations</li>
</ul>
<h2>mkdocs-material-9.0.10</h2>
<ul>
<li>Updated Arabic translations</li>
<li>Updated Korean translations</li>
<li>Updated Hungarian translations</li>
<li>Updated Russian translations</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4977">#4977</a>: Improved accessibility for content tabs</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4960">#4960</a>: Sometimes anchor following doesn't bring last item into view</li>
</ul>
<h2>mkdocs-material-9.0.9</h2>
<ul>
<li>Updated Bulgarian translations</li>
<li>Updated Chinese (Simplified) translations</li>
<li>Updated Dutch translations</li>
<li>Updated Hindi translations</li>
<li>Updated Japanese translations</li>
<li>Updated Polish translations</li>
</ul>
<h2>mkdocs-material-9.0.8</h2>
<ul>
<li>Updated Croatian translations</li>
<li>Updated French translations</li>
<li>Updated Hungarian translations</li>
<li>Updated Portuguese (Brasilian) translations</li>
<li>Updated Spanish translations</li>
<li>Updated Ukrainian translations</li>
<li>Updated Urdu translations</li>
<li>Updated Vietnamese translations</li>
</ul>
<h2>mkdocs-material-9.0.7</h2>
<ul>
<li>Improved accessibility of sidebar navigation</li>
<li>Moved all translations into community edition</li>
<li>Updated Polish and Portuguese (Brasilian) translations</li>
<li>Fixed info plugin terminating on subsequent reload when serving</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4910">#4910</a>: Sidebar navigation labels have invalid ARIA roles</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4884">#4884</a>: Search query terms can't be separated by colons</li>
</ul>
<h2>mkdocs-material-9.0.6</h2>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4883">#4883</a>: Automatically disable info plugin when serving</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4885">#4885</a>: Search plugin crashes in some exotic cases (9.0.3 regression)</li>
</ul>
<h2>mkdocs-material-9.0.5</h2>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4842">#4842</a>: Improved accessibility of search result list</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.0.12 (2023-02-09)</p>
<ul>
<li>Updated Catalan translations</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4975">#4975</a>: Mermaid entity relationship rendering diagrams bug</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4924">#4924</a>: Header title not reset when using instant loading</li>
</ul>
<p>mkdocs-material-9.0.11+insiders-4.30.0 (2023-02-06)</p>
<ul>
<li>Rewrite of privacy plugin for concurrency, now twice as fast</li>
<li>Added support for explicit inclusion for privacy plugin</li>
<li>Added optimization support for privacy plugin (+ optimize plugin)</li>
</ul>
<p>mkdocs-material-9.0.11 (2023-02-03)</p>
<ul>
<li>Added Mastodon verification for social links (rel=me)</li>
<li>Updated Italian translations</li>
</ul>
<p>mkdocs-material-9.0.10 (2023-02-02)</p>
<ul>
<li>Updated Arabic translations</li>
<li>Updated Korean translations</li>
<li>Updated Hungarian translations</li>
<li>Updated Russian translations</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4977">#4977</a>: Improved accessibility for content tabs</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4960">#4960</a>: Sometimes anchor following doesn't bring last item into view</li>
</ul>
<p>mkdocs-material-9.0.9 (2023-01-30)</p>
<ul>
<li>Updated Bulgarian translations</li>
<li>Updated Chinese (Simplified) translations</li>
<li>Updated Dutch translations</li>
<li>Updated Hindi translations</li>
<li>Updated Japanese translations</li>
<li>Updated Polish translations</li>
</ul>
<p>mkdocs-material-9.0.8 (2023-01-29)</p>
<ul>
<li>Updated Croatian translations</li>
<li>Updated French translations</li>
<li>Updated Hungarian translations</li>
<li>Updated Portuguese (Brasilian) translations</li>
<li>Updated Spanish translations</li>
<li>Updated Ukrainian translations</li>
<li>Updated Urdu translations</li>
<li>Updated Vietnamese translations</li>
</ul>
<p>mkdocs-material-9.0.7 (2023-01-28)</p>
<ul>
<li>Improved accessibility of sidebar navigation</li>
<li>Moved all translations into community edition</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/5e438cc0dbe68c2425d7baaf219aa0437bdab7cd"><code>5e438cc</code></a> Prepare 9.0.12 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/3a62681e37566a8bebe2e49440567f02e37eb8b6"><code>3a62681</code></a> Merge branch 'master' of github.com:squidfunk/mkdocs-material</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/ff99e19741158800edeeffa093330ab85711123a"><code>ff99e19</code></a> Fixed header title not reset on missing headline when using instant loading</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/803320f004345896c1a230bca6b2f8ef46ce41b9"><code>803320f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5020">#5020</a> from squidfunk/contributing/index</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/58d49fad66d26a75f19449508b0a56db26dd8ac5"><code>58d49fa</code></a> Updated index page</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/48e8b2be30fed05c76dda6bc20ff039ed3e8601f"><code>48e8b2b</code></a> Updated Catalan translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f7598410cba3af8dc184cdac7bcbb90394a4aab2"><code>f759841</code></a> Fixed attribute styles in entity-relationship diagrams</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/2e689f062f6f01bd7e20e850e92ec7811f719dea"><code>2e689f0</code></a> Updated issue template</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f60fa205f9d6719e4aea925619fac844d04e937e"><code>f60fa20</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5003">#5003</a> from squidfunk/issue/bug-report-update</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/83468bc6ed9378850c4569e9500a2b62bcb26991"><code>83468bc</code></a> Updated links in bug report</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.0.0...9.0.12">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.0.0&new-version=9.0.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 22:43:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1265" class=".btn">#1265</a>
            </td>
            <td>
                <b>
                    Add Sirato Explorer docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexandra Tran <alexandra.tran@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

Add Sirato Blockchain Explorer docs. This PR replaces #1252, which has significant multi-contributor DCO errors.

Migrate the original content from that PR and edit and restructure it.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

For tool changes:

- [ ] Github Actions workflow
- [ ] Build and QA tools configuration (for example, lint rules or Vale style)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [ ] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 19:58:42 +0000 UTC
    </div>
</div>

