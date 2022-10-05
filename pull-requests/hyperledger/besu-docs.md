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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 8.3.9 to 8.5.6 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 8.3.9 to 8.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-8.5.6</h2>
<ul>
<li>Modernized appearance of admonitions (with fallback, see <a href="https://squidfunk.github.io/mkdocs-material/reference/admonitions/#classic-admonitions">docs</a>)</li>
<li>Improved appearance of inline code blocks in admonition titles</li>
</ul>
<h2>mkdocs-material-8.5.5</h2>
<ul>
<li>Updated MkDocs to 1.4</li>
<li>Fixed compatibility issues with MkDocs 1.4</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4430">#4430</a>: build error when enabling consent without repository URL</li>
</ul>
<h2>mkdocs-material-8.5.4</h2>
<ul>
<li>Fixed expand icons shift on sidebar overflow (using <code>scrollbar-gutter</code>)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4429">#4429</a>: Text in sequence diagrams overflows in Firefox</li>
</ul>
<h2>mkdocs-material-8.5.3</h2>
<ul>
<li>Fixed build error when enabling cookie consent without analytics</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4381">#4381</a>: Code blocks render ligatures for some fonts</li>
</ul>
<h2>mkdocs-material-8.5.2</h2>
<ul>
<li>Updated Mermaid.js to version 9.1.7</li>
<li>Fixed overly large headlines in search results (8.5.0 regression)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4358">#4358</a>: Navigation sections appear as clickable (8.5.0 regression)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4356">#4356</a>: GitHub repository statistics fetched before consent</li>
</ul>
<h2>mkdocs-material-8.5.1</h2>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4366">#4366</a>: Removed dependencies with native extensions</li>
</ul>
<h2>mkdocs-material-8.5.0</h2>
<ul>
<li>Added support for social cards</li>
<li>Added support for code annotation anchor links (deep linking)</li>
<li>Added support for code annotation comment stripping (syntax modifier)</li>
<li>Added support for sidebars scrolling automatically to active item</li>
<li>Added support for anchor following table of contents (= auto scroll)</li>
<li>Added support for tag icons</li>
</ul>
<h2>mkdocs-material-8.4.4</h2>
<ul>
<li>Moved comments integration to separate partial (<code>comments.html</code>)</li>
</ul>
<h2>mkdocs-material-8.4.3</h2>
<ul>
<li>Added Simple Icons to bundled icons (+2,300 icons)</li>
<li>Added support for changing edit icon</li>
<li>Moved page actions to separate partial (<code>actions.html</code>)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4291">#4291</a>: Version switching doesn't stay on page when anchors are used</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4327">#4327</a>: Links in data tables do not receive link styling</li>
</ul>
<h2>mkdocs-material-8.4.2</h2>
<ul>
<li>Updated Slovenian translations</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4277">#4277</a>: Feedback widget hidden after navigation with instant loading</li>
<li>Fixed numeric tags in front matter breaking search functionality</li>
</ul>
<h2>mkdocs-material-8.4.1</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-8.5.6+insiders-4.25.2 (2022-10-04)</p>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4452">#4452</a>: Blog and tags plugin crash when specifying slugify function</li>
</ul>
<p>mkdocs-material-8.5.6+insiders-4.25.1 (2022-10-03)</p>
<ul>
<li>Updated mkdocs-rss-plugin in Dockerfile to fix MkDocs compat errors</li>
</ul>
<p>mkdocs-material-8.5.6+insiders-4.25.0 (2022-10-02)</p>
<ul>
<li>Added support for navigation subtitles</li>
<li>Added support for defining an allow list for built-in tags plugin</li>
<li>Added support for custom slugify functions for built-in tags plugin</li>
<li>Improved stability of search plugin when using --dirtyreload</li>
</ul>
<p>mkdocs-material-8.5.6 (2022-10-02)</p>
<ul>
<li>Modernized appearance of admonitions (with fallback, see docs)</li>
<li>Improved appearance of inline code blocks in admonition titles</li>
</ul>
<p>mkdocs-material-8.5.5+insiders-4.24.2 (2022-10-01)</p>
<ul>
<li>Updated MkDocs to 1.4</li>
<li>Fixed compatibility issues with MkDocs 1.4</li>
<li>Fixed incorrectly generated paths in privacy plugin</li>
<li>Fixed blog index page not showing navigation when using meta plugin</li>
</ul>
<p>mkdocs-material-8.5.5 (2022-10-01)</p>
<ul>
<li>Updated MkDocs to 1.4</li>
<li>Fixed compatibility issues with MkDocs 1.4</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4430">#4430</a>: build error when enabling consent without repository URL</li>
</ul>
<p>mkdocs-material-8.5.4+insiders-4.24.1 (2022-09-30)</p>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4430">#4430</a>: build error when enabling consent without repository URL</li>
</ul>
<p>mkdocs-material-8.5.4 (2022-09-30)</p>
<ul>
<li>Fixed expand icons shift on sidebar overflow (using scrollbar-gutter)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4429">#4429</a>: Text in sequence diagrams overflows in Firefox</li>
</ul>
<p>mkdocs-material-8.5.3+insiders-4.24.0 (2022-09-27)</p>
<ul>
<li>Added support for custom content on index pages (blog)</li>
<li>Added support for keeping content on paginated index pages (blog)</li>
<li>Added support for limiting categories in post excerpts (blog)</li>
<li>Added support for simple override of templates via front matter (blog)</li>
<li>Added icon in navigation for pages with encrypted content</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4396">#4396</a>: Front matter of index pages not inherited by pagination (blog)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f139b54c61b2df4512f15149cba2c222475e2bc9"><code>f139b54</code></a> Prepare 8.5.6 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/d1fc8598212532a58c924a43f18b8f1fa8a096d3"><code>d1fc859</code></a> Prepare 8.5.6 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/c44baee78d5cffec89c5d39c79b6504609795331"><code>c44baee</code></a> Documentation</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/ee1e675da613fb26b71d0385f732a55eac6aea73"><code>ee1e675</code></a> Update slug reference</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/29f00a5bb8edabddaf2d6d211434b59bdde25c3d"><code>29f00a5</code></a> Modernized look of admonitions</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/6edbcf896833026667149c47514542a8c438d490"><code>6edbcf8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4392">#4392</a> from squidfunk/pin</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/1e508d6292a5b7fb7e57ddea75b0c672e0a4ffc5"><code>1e508d6</code></a> Documentation</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/0a5ab025b5a356facb6d2fc3b1bbbe1e4b6e806c"><code>0a5ab02</code></a> Updated documentation and fixed syntax error in schema</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/cec89f0c6dd95fb6c6c6f2ae17551090f5639f1d"><code>cec89f0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4303">#4303</a> from ojacques/master</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/26b307070ad60d2bc4a103ef4c0d27a1d888d62f"><code>26b3070</code></a> Updated Insiders changelog</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/8.3.9...8.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=8.3.9&new-version=8.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-10-05 17:08:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    Bump plantuml-markdown from 3.6.2 to 3.6.3 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [plantuml-markdown](https://github.com/mikitex70/plantuml-markdown) from 3.6.2 to 3.6.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/releases">plantuml-markdown's releases</a>.</em></p>
<blockquote>
<h2>Fixed rendering of yaml structures with remote server</h2>
<p>When rendering plantuml yaml diagrams on a remote server, the spaces were removed from the lines and the diagram was not drawn as expected.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/blob/master/CHANGELOG.md">plantuml-markdown's changelog</a>.</em></p>
<blockquote>
<h2>3.6.3 (2022-08-01)</h2>
<h3>Fix</h3>
<ul>
<li>
<p>Removed unused <code>plantuml</code> import. [Michele Tessaro]</p>
</li>
<li>
<p>Doc: fix typos. [Kian-Meng Ang]</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/0f214940f663f6524ab42aa1e2d792a15f026b23"><code>0f21494</code></a> Merge branch 'develop'</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/55170a11d5d0d7ee814b10cead80d7bbfc89f83b"><code>55170a1</code></a> fix: usr: fixed yaml renderingwith remote server (fixes <a href="https://github-redirect.dependabot.com/mikitex70/plantuml-markdown/issues/72">#72</a>)</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/9f968f6fccf7651d0054c6234eb789154a94a417"><code>9f968f6</code></a> fix: usr: removed unused <code>plantuml</code> import</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/873eeedb1323230c4355585630f9d6b3ad96836a"><code>873eeed</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mikitex70/plantuml-markdown/issues/62">#62</a> from kianmeng/fix-typos</li>
<li>See full diff in <a href="https://github.com/mikitex70/plantuml-markdown/compare/3.6.2...3.6.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=plantuml-markdown&package-manager=pip&previous-version=3.6.2&new-version=3.6.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-10-05 17:08:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1184" class=".btn">#1184</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-redirects from 1.0.4 to 1.2.0 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-redirects](https://github.com/datarobot/mkdocs-redirects) from 1.0.4 to 1.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/datarobot/mkdocs-redirects/releases">mkdocs-redirects's releases</a>.</em></p>
<blockquote>
<h2>v1.2.0</h2>
<ul>
<li>
<p>For better interoperability with plugins, the redirect target paths are picked up from the corresponding MkDocs <code>File</code> and not re-computed by simple substitution. (<a href="https://github-redirect.dependabot.com/datarobot/mkdocs-redirects/issues/45">#45</a>)</p>
</li>
<li>
<p>Drop Python 2.7 support</p>
</li>
<li>
<p>Bump minimal MkDocs version to 1.1.1</p>
</li>
<li>
<p>Remove warning about old <code>redirects</code> config</p>
</li>
</ul>
<h2>v1.1.0</h2>
<ul>
<li>
<p>Redirect destination paths can now contain #fragments (<a href="https://github-redirect.dependabot.com/datarobot/mkdocs-redirects/issues/42">#42</a>)</p>
<p>Example config:</p>
<pre lang="yaml"><code>plugins:
  - redirects:
      redirect_maps:
        some/path/examples.md: foo/index.md#examples
</code></pre>
<p>-- this will now correctly redirect to <code>foo/#examples</code> without messing up the path</p>
<p>Note that this applies only to the <em>destination</em> paths, there's still no handling for fragments in <em>source</em> paths (those specified as map keys).</p>
</li>
</ul>
<h2>v1.0.6</h2>
<ul>
<li>Correctly use UTF-8 file encoding even on Windows (<a href="https://github-redirect.dependabot.com/datarobot/mkdocs-redirects/issues/41">#41</a>)</li>
</ul>
<h2>v1.0.5</h2>
<ul>
<li>Normalize only capitalized <code>README.md</code> files to <code>index</code> (<a href="https://github-redirect.dependabot.com/datarobot/mkdocs-redirects/issues/37">#37</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/ad6769c70d7d60ef6cc7589ad86f99b25639e296"><code>ad6769c</code></a> Release 1.2.0 (<a href="https://github-redirect.dependabot.com/datarobot/mkdocs-redirects/issues/48">#48</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/106ced625f2f8dc97965b6a8c8920e42d3fb544e"><code>106ced6</code></a> Test redirect to absolute URL</li>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/152f7375fbf91ddb5a9f4dc383fd8e84178ac088"><code>152f737</code></a> Remove unneeded code path</li>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/30ce6c3107293aa9a0c7b3d042bb365790b4d272"><code>30ce6c3</code></a> Refactor: put the string template as a constant</li>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/3dc57eb655bd31837caaccad81b8f9c0c4a49949"><code>3dc57eb</code></a> Refactor get_html_path: use implementation from MkDocs</li>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/577c0e23a94bcca0d5e6a20bef52b6a03a1b5e63"><code>577c0e2</code></a> Add a test for a file with a custom <code>url</code></li>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/657aa51d70b80e4789b5a46927433e1db8544e00"><code>657aa51</code></a> Also test the left side of the redirect</li>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/a81e0641927ec0b59625b24effb2906b5c694d81"><code>a81e064</code></a> Refactor the test to be more end-to-end</li>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/5d05d15dac38628edd730b6b21aa78e4c288a8c9"><code>5d05d15</code></a> Merge two test cases into one</li>
<li><a href="https://github.com/mkdocs/mkdocs-redirects/commit/c80e4877db975eaaeaa357aac570fefa4cba5738"><code>c80e487</code></a> CI: Enforce black+isort+autoflake</li>
<li>Additional commits viewable in <a href="https://github.com/datarobot/mkdocs-redirects/compare/v1.0.4...v1.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-redirects&package-manager=pip&previous-version=1.0.4&new-version=1.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-10-05 17:08:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1183" class=".btn">#1183</a>
            </td>
            <td>
                <b>
                    try gitleaks again
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

add gitleaks config to exclude test secrets

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

## Issue fixed

fixes https://github.com/github/super-linter/issues/3407

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [ ] Documentation content
- [ ] Documentation page organization

For tool changes:

- [x] Github Actions workflow
- [x] Build and QA tools configuration (for example, lint rules or Vale style)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
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
        Created At 2022-10-05 14:06:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1182" class=".btn">#1182</a>
            </td>
            <td>
                <b>
                    Document `--tx-pool-future-max-by-account`
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

Document `--tx-pool-future-max-by-acount` cli option.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

fixes #1154 

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
        Created At 2022-10-04 20:55:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1181" class=".btn">#1181</a>
            </td>
            <td>
                <b>
                    Update `--fast-sync-min-peers` default value
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

Update docs on `--fast-sync-min-peers` default value from 5 to 1.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

fixes #1155 

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
        Created At 2022-10-04 20:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1180" class=".btn">#1180</a>
            </td>
            <td>
                <b>
                    fix code blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Signed-off-by: Nicolas MASSART <NicolasMassart@users.noreply.github.com>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Code blocks were broken (too much increment)

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

## Issue fixed

- Fixed the code blocks
- disabled the secret linter as it doesn't work properly when we have test secrets in the doc. See https://github.com/github/super-linter/issues/3407
- made the linter option value consistently unquoted

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

- [x] Github Actions workflow
- [x] Build and QA tools configuration (for example, lint rules or Vale style)
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

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->
https://hyperledger-besu--1180.org.readthedocs.build/en/1180/private-networks/tutorials/permissioning/onchain/#11-clone-the-contracts-and-install-dependencies
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-03 14:15:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1179" class=".btn">#1179</a>
            </td>
            <td>
                <b>
                    Post-merge updates to match Teku docs
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

Minor updates to merge/getting started content to be consistent with recent updates to Teku docs.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

fixes #1178 

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
        Created At 2022-10-02 02:50:51 +0000 UTC
    </div>
</div>

