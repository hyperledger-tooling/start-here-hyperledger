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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1325" class=".btn">#1325</a>
            </td>
            <td>
                <b>
                    Add missing quotes in trace call example
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
- [ ]  You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Fix trace_call json example - missing double quotes in the start of the field "to".

Preview:
https://hyperledger-besu--1325.org.readthedocs.build/en/1325/public-networks/reference/api/?h=trace+call#trace_call

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
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 04:52:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1324" class=".btn">#1324</a>
            </td>
            <td>
                <b>
                    python version bump
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Projects using read the docs: you need to update your .readthedocs.yml to look like this: https://github.com/hyperledger/cacti/blob/10746c3e65891dfa38658d9ecae631222b92fddd/.readthedocs.yaml urllib released which broke previous configs. https://github.com/readthedocs/readthedocs.org/issues/10290 https://www.reddit.com/r/technicalwriting/comments/138rxms/readthedocs_sphinx_theme_urllib3_related_build/

For content changes:

- [ ] Documentation content
- [ ] Documentation page organization

For tool changes:

- [ ] Github Actions workflow
- [ ] Build and QA tools configuration (for example, lint rules or Vale style)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [x] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [ ] You've fixed any issues raised by the tests.
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
        Created At 2023-05-10 03:46:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1322" class=".btn">#1322</a>
            </td>
            <td>
                <b>
                    Unix timestamp (milliseconds)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1321 

- [x] Documentation content
- [ ] Documentation page organization


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 02:27:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1320" class=".btn">#1320</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 9.1.8 to 9.1.11 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.1.8 to 9.1.11.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.1.11</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5487">#5487</a>: Social plugin crashes without options (9.1.10 regression)</li>
</ul>
<h2>mkdocs-material-9.1.10</h2>
<ul>
<li>Added <code>cards_layout_options</code> setting for social cards</li>
<li>Deprecated <code>cards_color</code> and <code>cards_font</code> setting for social cards</li>
</ul>
<h2>mkdocs-material-9.1.9</h2>
<ul>
<li>Added Telugu, Kannada and Sanskrit translations</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5428">#5428</a>: Fixed margins for light/dark mode images in figures</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5420">#5420</a>: Social plugin crashing for some specific Google Fonts</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5160">#5160</a>: Instant loading makes code annotations jump (9.1.1 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/4920">#4920</a>: Social plugin not loading logo from custom icon set</li>
<li>Fixed social plugin crashing when only code font is specified</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.1.11 (2023-05-08)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5487">#5487</a>: Social plugin crashes without options (9.1.10 regression)</li>
</ul>
<p>mkdocs-material-9.1.10+insiders-4.33.0 (2023-05-08)</p>
<ul>
<li>Added support for custom layouts for social plugin</li>
<li>Added support for background images for social cards</li>
</ul>
<p>mkdocs-material-9.1.10 (2023-05-08)</p>
<ul>
<li>Added cards_layout_options setting for social cards</li>
<li>Deprecated cards_color and cards_font setting for social cards</li>
</ul>
<p>mkdocs-material-9.1.9 (2023-05-02)</p>
<ul>
<li>Added Telugu, Kannada and Sanskrit translations</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5428">#5428</a>: Fixed margins for light/dark mode images in figures</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5420">#5420</a>: Social plugin crashing for some specific Google Fonts</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5160">#5160</a>: Instant loading makes code annotations jump (9.1.1 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/4920">#4920</a>: Social plugin not loading logo from custom icon set</li>
<li>Fixed social plugin crashing when only code font is specified</li>
</ul>
<p>mkdocs-material-9.1.8 (2023-04-24)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5417">#5417</a>: Theme breaks when palette is not defined (9.1.7 regression)</li>
</ul>
<p>mkdocs-material-9.1.7+insiders-4.32.6 (2023-04-22)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5336">#5336</a>: Interplay of blog plugin with git-revision-date-localized</li>
</ul>
<p>mkdocs-material-9.1.7 (2023-04-22)</p>
<ul>
<li>Updated Persian (Farsi) and Turkish translations</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5401">#5401</a>: Added missing flag to disable built-in tags plugin</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5206">#5206</a>: Ensure defaults are set for primary and accent colors</li>
<li>Fixed unnecessary inclusion of palette CSS when unused</li>
</ul>
<p>mkdocs-material-9.1.6+insiders-4.32.5 (2023-04-07)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5322">#5322</a>: Navigation tabs hoist nested page icons</li>
</ul>
<p>mkdocs-material-9.1.6 (2023-04-07)</p>
<ul>
<li>Updated Persian (Farsi) translations</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5300">#5300</a>: Boxes in Mermaid sequence diagrams not color-abiding</li>
</ul>
<p>mkdocs-material-9.1.5 (2023-03-31)</p>
<ul>
<li>Updated Lithuanian and Japanese translations</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/85de63f68397db94bc047a9375a1b02e401679fa"><code>85de63f</code></a> Updated changelog</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/c91174f23819ff84c640cf9c91bff181fcf946c2"><code>c91174f</code></a> Prepare 9.1.11 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/8b50290f5e2f4dcc35264deae2f88fd82106bfbf"><code>8b50290</code></a> Fixed errors in deprecation path of social plugin settings</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/b0d59f2241baaa380468614ae0b8880f4c6ca9e8"><code>b0d59f2</code></a> Documentation</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/5b9f6c972dc85e1060a52057a3e9a7c8053822dd"><code>5b9f6c9</code></a> Updated changelog</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/b4dd4491e9625af1c633ab5db56bb9648f3b3324"><code>b4dd449</code></a> Prepare 9.1.10 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/09feabc579a1b67dc906e3d8582076acec36b9ec"><code>09feabc</code></a> Harmonized color and font settings for social cards with Insiders</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/2735c87d9ad380480c693773c42c759dee340f88"><code>2735c87</code></a> Finished documentation on social cards</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/8a8662c340d7ff696989142caf6d0769ed09e333"><code>8a8662c</code></a> Merge branch 'master' into docs/social-cards</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/64bbaff541af3d80d97a4ef13ef7c8e9c0b5a50b"><code>64bbaff</code></a> Merge branch 'master' of github.com:squidfunk/mkdocs-material</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.1.8...9.1.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.1.8&new-version=9.1.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-05-08 23:58:01 +0000 UTC
    </div>
</div>

