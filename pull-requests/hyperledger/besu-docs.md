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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1233" class=".btn">#1233</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 8.5.11 to 9.0.0 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 8.5.11 to 9.0.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.0.0</h2>
<p><strong>Additions and improvements</strong></p>
<ul>
<li>Added support for rich search previews</li>
<li>Added support for tokenizer lookahead</li>
<li>Added support for better search highlighting</li>
<li>Added support for excluding content from search</li>
<li>Added support for configurable search pipeline</li>
<li>Added support for offline search via offline plugin</li>
<li>Added support for multiple instances of built-in tags plugin</li>
<li>Added support for removing copy-to-clipboard button</li>
<li>Added support for removing footer navigation</li>
<li>Added support for button to view the source of a page</li>
<li>Improved readability of query string for search sharing</li>
<li>Improved stability of search plugin when using <code>--dirtyreload</code></li>
<li>Improved search result group button, now sticky and stable</li>
<li>Updated Norwegian translations</li>
<li>Updated MkDocs to 1.4.2</li>
</ul>
<p><strong>Removals</strong></p>
<ul>
<li>Removed deprecated alternative admonition qualifiers</li>
<li>Removed <code>:is()</code> selectors (in output) for easier overriding</li>
<li>Removed <code>.title</code> suffix on translations</li>
<li>Removed legacy method for providing page title in feedback URL</li>
<li>Removed support for indexing only titles in search</li>
<li>Removed support for custom search transforms</li>
<li>Removed support for custom search workers</li>
<li>Removed temporary snow feature (easter egg)</li>
</ul>
<p><strong>Fixes</strong></p>
<ul>
<li>Fixed Norwegian and Korean language code</li>
<li>Fixed detection of composition events in search interface</li>
<li>Fixed search plugin not using title set via front matter</li>
<li>Fixed search highlighting of tags</li>
<li>Fixed search sharing URL using post transformed string</li>
<li>Fixed theme-color meta tag getting out-of-sync with palette toggle</li>
<li>Fixed prev/next page keyboard navigation when footer is not present</li>
<li>Fixed overflowing navigation tabs not being scrollable</li>
<li>Fixed inclusion of code block line numbers from search</li>
</ul>
<h2>mkdocs-material-9.0.0b4</h2>
<p><strong>Note: this is a beta release</strong> – see <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4714">#4714</a></p>
<ul>
<li>Improved readability of search sharing link</li>
<li>Fixed search highlighting of occurrences found in tags</li>
<li>Fixed search sharing link using post transformed string (with wildcards etc.)</li>
<li>Fixed inability to query specific fields (e.g. <code>tags:foo</code> or <code>title:bar</code>)</li>
<li>Fixed inability to exclude search terms (e.g. <code>-foo</code> or <code>-title:bar</code>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.x.x</p>
<ul>
<li>Removed pipdeptree dependency for info plugin</li>
<li>Fixed appearance of linked tags when hovered (9.0.0 regression)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4810">#4810</a>: Abbreviations run out of screen on touch devices</li>
</ul>
<p>mkdocs-material-9.0.0 (2023-01-02)</p>
<p>Additions and improvements</p>
<ul>
<li>Added support for rich search previews</li>
<li>Added support for tokenizer lookahead</li>
<li>Added support for better search highlighting</li>
<li>Added support for excluding content from search</li>
<li>Added support for configurable search pipeline</li>
<li>Added support for offline search via offline plugin</li>
<li>Added support for multiple instances of built-in tags plugin</li>
<li>Added support for removing copy-to-clipboard button</li>
<li>Added support for removing footer navigation</li>
<li>Added support for button to view the source of a page</li>
<li>Improved readability of query string for search sharing</li>
<li>Improved stability of search plugin when using --dirtyreload</li>
<li>Improved search result group button, now sticky and stable</li>
<li>Updated Norwegian translations</li>
<li>Updated MkDocs to 1.4.2</li>
</ul>
<p>Removals</p>
<ul>
<li>Removed deprecated alternative admonition qualifiers</li>
<li>Removed :is() selectors (in output) for easier overriding</li>
<li>Removed .title suffix on translations</li>
<li>Removed legacy method for providing page title in feedback URL</li>
<li>Removed support for indexing only titles in search</li>
<li>Removed support for custom search transforms</li>
<li>Removed support for custom search workers</li>
<li>Removed temporary snow feature (easter egg)</li>
</ul>
<p>Fixes</p>
<ul>
<li>Fixed Norwegian and Korean language code</li>
<li>Fixed detection of composition events in search interface</li>
<li>Fixed search plugin not using title set via front matter</li>
<li>Fixed search highlighting of tags</li>
<li>Fixed search sharing URL using post transformed string</li>
<li>Fixed theme-color meta tag getting out-of-sync with palette toggle</li>
<li>Fixed prev/next page keyboard navigation when footer is not present</li>
<li>Fixed overflowing navigation tabs not being scrollable</li>
<li>Fixed inclusion of code block line numbers from search</li>
</ul>
<p>mkdocs-material-8.5.11+insiders-4.27.0 (2022-12-20)</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Upgrade guide</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/docs/upgrade.md">mkdocs-material's upgrade guide</a>.</em></p>
<blockquote>
<h1>How to upgrade</h1>
<p>Upgrade to the latest version with:</p>
<pre><code>pip install --upgrade --force-reinstall mkdocs-material
</code></pre>
<p>Show the currently installed version with:</p>
<pre><code>pip show mkdocs-material
</code></pre>
<h2>Upgrading from 8.x to 9.x</h2>
<p>This major release includes a brand new search implementation that is faster
and allows for rich previews, advanced tokenization and better highlighting.
It was available as part of Insiders for over a year, and now that the funding
goal was hit, makes its way into the community edition.</p>
<h3>Changes to <code>mkdocs.yml</code></h3>
<h4><code>content.code.copy</code></h4>
<p>The copy-to-clipboard buttons are now opt-in and can be enabled or disabled
per block. If you wish to enable them for all code blocks, add the following
lines to <code>mkdocs.yml</code>:</p>
<pre lang="yaml"><code>theme:
  features:
    - content.code.copy
</code></pre>
<h4><code>content.action.*</code></h4>
<p>A &quot;view source&quot; button can be shown next to the &quot;edit this page&quot; button, both
of which must now be explicitly enabled. Add the following lines to
<code>mkdocs.yml</code>:</p>
<pre lang="yaml"><code>theme:
  features:
    - content.action.edit
    - content.action.view
</code></pre>
<h4><code>navigation.footer</code></h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/b95dffa5cd7c32a443ab2c46d63252bc828409ec"><code>b95dffa</code></a> Removed level 1 headline hack in content partial</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/39013249a50ae0bcac7f2b32ccee4c0947abf0c6"><code>3901324</code></a> Updated .gitignore</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/3b921f76a3bb268f169dd800ba59bbad7dedeb83"><code>3b921f7</code></a> Updated copyright year</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/d25326fc520a62ea958095c6010b1c80cc58dbc3"><code>d25326f</code></a> Updated site description in mkdocs.yml</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/1b08038f866da3d15614ad28fcf0f63a13aaa076"><code>1b08038</code></a> Removed patch-level version spec where not necessary</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/01b25dddcb6f6c7932b95f53587c399fbb50fc98"><code>01b25dd</code></a> Improved platform information in info plugin</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/fc6a368d6b37ca558cf06a3f6cfb6403b5222e23"><code>fc6a368</code></a> Fixed alternative fragments in Mermaid diagrams</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/23730a1f150d25d8fa899417d6cba02139650793"><code>23730a1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4628">#4628</a> from squidfunk/feature/material-v9</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/a8c8583c5c7160a5973677e013aa83b981c707ba"><code>a8c8583</code></a> Fixed hatch</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/1295539ec23f35dd22a5a6643fd4ae0429e92b2a"><code>1295539</code></a> Added back hatch for release management</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/8.5.11...9.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=8.5.11&new-version=9.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-02 23:03:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1232" class=".btn">#1232</a>
            </td>
            <td>
                <b>
                    Bump plantuml-markdown from 3.7.3 to 3.8.0 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [plantuml-markdown](https://github.com/mikitex70/plantuml-markdown) from 3.7.3 to 3.8.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/releases">plantuml-markdown's releases</a>.</em></p>
<blockquote>
<h2>Minor enhancements</h2>
<ul>
<li>added <code>preserveAspectRatio</code> to inline SVGs to keep aspect ratio when the diagram is resized</li>
<li>added <code>id</code> attribute to images to simplify referencing in CSS rules or Javascript code</li>
<li>added option to disable the removal of inline SVG size (see <a href="https://github-redirect.dependabot.com/mikitex70/plantuml-markdown/issues/81">#81</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/blob/master/CHANGELOG.md">plantuml-markdown's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>development (unreleased)</h2>
<h3>New</h3>
<ul>
<li>
<p>Added <code>preserveAspectRatio</code> to inline SVG diagrams. [Michele Tessaro]</p>
</li>
<li>
<p>Added <code>id</code> diagram option. [Michele Tessaro]</p>
<p>When the <code>id</code> option is used, an <code>id</code> attribute will be generated for the
diagram.
This can be useful for referencing the diagram in CSS rules or
Javascript code.</p>
</li>
<li>
<p>Added <code>remove_inline_svg_size</code> config option. [Anders Norman]</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/6f36347caa01b549f8f2a80fb84632bab10363ea"><code>6f36347</code></a> chg: dev: prepared for the new release</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/fdc873913b227b84587c8f5f1216dce7108fed39"><code>fdc8739</code></a> new: usr: added <code>preserveAspectRatio</code> to inline SVG diagrams</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/0ce98542c2202e5063958e53ef79f5ccdd29fb94"><code>0ce9854</code></a> new: usr: added <code>id</code> diagram option</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/386458c647a6a29c95487985c6159332fe8a7649"><code>386458c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mikitex70/plantuml-markdown/issues/82">#82</a> from anorm/remove_inline_svg_size</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/d606db3b5cbc3ca5e05bdf6dcf8e494bbc208364"><code>d606db3</code></a> Added 'remove_inline_svg_size' config option</li>
<li>See full diff in <a href="https://github.com/mikitex70/plantuml-markdown/compare/3.7.3...3.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=plantuml-markdown&package-manager=pip&previous-version=3.7.3&new-version=3.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-02 23:03:42 +0000 UTC
    </div>
</div>

