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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1284" class=".btn">#1284</a>
            </td>
            <td>
                <b>
                    changing page to reflect we will not be implementing forest snap server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                see change details - "to be implemented" --> "No" 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 00:39:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1283" class=".btn">#1283</a>
            </td>
            <td>
                <b>
                    Bump plantuml-markdown from 3.8.0 to 3.8.2 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [plantuml-markdown](https://github.com/mikitex70/plantuml-markdown) from 3.8.0 to 3.8.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/releases">plantuml-markdown's releases</a>.</em></p>
<blockquote>
<p>Forced UTF-8 encoding when files are passed to local plantuml.
Make sure that the diagram files are in utf-8, especially in Windows.</p>
<h2>Added option for disabling SSL checks</h2>
<p>Added the 'insecure<code>configuration option to disable HTTPS SSL certificate validation. Set to</code>True` when using a custom PlantUML installation with self-signed certificates.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/blob/master/CHANGELOG.md">plantuml-markdown's changelog</a>.</em></p>
<blockquote>
<h2>3.8.2 (2023-03-06)</h2>
<h3>Changes</h3>
<ul>
<li>Updated CHANGELOG for the new release. [Michele Tessaro]</li>
</ul>
<h3>Fix</h3>
<ul>
<li>
<p>Explicitly pass charset to plantuml. [Victor Westerhuis]</p>
<p>The code is explicitly encoded to UTF-8, but plantuml gets to pick its own charset. On my Windows installation it picks codepage 1252 by default, leading to wrong characters in the output. UTF-8 should be available everywhere according to the <a href="https://plantuml.com/unicode">PlantUML documentation</a>.</p>
</li>
</ul>
<h2>3.8.1 (2023-01-29)</h2>
<h3>New</h3>
<ul>
<li>
<p>Added option for disabling SSL checks (refs <a href="https://github-redirect.dependabot.com/mikitex70/plantuml-markdown/issues/83">#83</a>) [Michele Tessaro]</p>
<p>Added the <code>insecure</code> configuration option for disabling HTTPS SSL
certificate validation.
Set it to <code>True</code> when the PlantUML server uses self-signed certificates.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/e48b04918315d769d91b4714f111f3f90668c872"><code>e48b049</code></a> chg: pkg: changed version for the new release</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/81c4b0300ffdfaf588db5e430759b8a0fdd24338"><code>81c4b03</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mikitex70/plantuml-markdown/issues/85">#85</a> from viccie30/patch-1</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/4d366fc946c9593d4993c84a8869849985b6b99c"><code>4d366fc</code></a> Explicitly pass charset to plantuml</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/d63efae88ac519d21b2c614090b380208fb76554"><code>d63efae</code></a> chg: doc: updated CHANGELOG for the new release</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/79d5f7ba9ee9d7e98921ce1a1b09520da21de696"><code>79d5f7b</code></a> new: usr: added option for disabling SSL checks (refs <a href="https://github-redirect.dependabot.com/mikitex70/plantuml-markdown/issues/83">#83</a>)</li>
<li>See full diff in <a href="https://github.com/mikitex70/plantuml-markdown/compare/3.8.0...3.8.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=plantuml-markdown&package-manager=pip&previous-version=3.8.0&new-version=3.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-03-07 00:01:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1282" class=".btn">#1282</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 9.0.0 to 9.1.1 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.0.0 to 9.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.1.1</h2>
<ul>
<li>Updated Czech and Thai translations</li>
<li>Improved instant loading (scroll restoration, slow connections)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5023">#5023</a>: Instant loading not allowing to go back to initial page</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/3797">#3797</a>: Instant loading does not work with section anchors in Safari</li>
</ul>
<h2>mkdocs-material-9.1.0</h2>
<ul>
<li>Docker image now available for <code>amd64</code>, <code>arm64</code> and <code>arm/v7</code></li>
<li>Updated Chinese (Taiwanese) translations</li>
<li>Generalized tag identifier implementation</li>
<li>Fixed flickering of header shadow on load</li>
<li>Fixed occasional flickering of announcement bar</li>
</ul>
<h2>mkdocs-material-9.0.15</h2>
<ul>
<li>Updated Chinese (Traditional) translations</li>
<li>Updated Hebrew translations</li>
</ul>
<h2>mkdocs-material-9.0.14</h2>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5072">#5072</a>: Rendering bug on navigation expand button in Firefox</li>
</ul>
<h2>mkdocs-material-9.0.13</h2>
<ul>
<li>Updated Uzbek translations</li>
<li>Switched back to pre-9.0.0 headline detection in <code>content</code> partial</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5062">#5062</a>: Version warning not readable when using slate scheme</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5061">#5061</a>: Improved discernibility of table row hover color</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5034">#5034</a>: Sequence actors in Mermaid diagrams not color-abiding</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4919">#4919</a>: Allow to hide version warning in multiple versions</li>
</ul>
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
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.1.1 (2023-03-05)</p>
<ul>
<li>Updated Czech and Thai translations</li>
<li>Improved instant loading (scroll restoration, slow connections)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5023">#5023</a>: Instant loading not allowing to go back to initial page</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/3797">#3797</a>: Instant loading does not work with section anchors in Safari</li>
</ul>
<p>mkdocs-material-9.1.0+insiders-4.32.2 (2023-03-02)</p>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5127">#5127</a>: Privacy plugin not handling large number of occurrences</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5126">#5126</a>: Privacy plugin breaks when replacing specific emojis</li>
</ul>
<p>mkdocs-material-9.1.0 (2023-03-02)</p>
<ul>
<li>Docker image now available for amd64, arm64 and arm/v7</li>
<li>Updated Chinese (Taiwanese) translations</li>
<li>Generalized tag identifier implementation</li>
<li>Fixed flickering of header shadow on load</li>
<li>Fixed occasional flickering of announcement bar</li>
</ul>
<p>mkdocs-material-9.0.15 (2023-02-26)</p>
<ul>
<li>Updated Chinese (Traditional) translations</li>
<li>Updated Hebrew translations</li>
</ul>
<p>mkdocs-material-9.0.14+insiders-4.32.1 (2023-02-23)</p>
<ul>
<li>Fixed code block spans interfering with copying</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5077">#5077</a>: Privacy plugin breaks image alt text encoding</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5079">#5079</a>: Privacy plugin removing rel=me on external links</li>
</ul>
<p>mkdocs-material-9.0.14 (2023-02-23)</p>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5072">#5072</a>: Rendering bug on navigation expand button in Firefox</li>
</ul>
<p>mkdocs-material-9.0.13+insiders-4.32.0 (2023-02-19)</p>
<ul>
<li>Added support for custom selectors for code annotations</li>
<li>Added support for code line range selection for better sharing</li>
</ul>
<p>mkdocs-material-9.0.13+insiders-4.31.0 (2023-02-18)</p>
<ul>
<li>Added support for table of contents on blog index and archive pages</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4512">#4512</a>: Allow custom search field boosts (experimental)</li>
</ul>
<p>mkdocs-material-9.0.13 (2023-02-18)</p>
<ul>
<li>Updated Uzbek translations</li>
<li>Switched back to pre-9.0.0 headline detection in content partial</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5062">#5062</a>: Version warning not readable when using slate scheme</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/2eff27fb2bfd09371301794d050fff7a22229902"><code>2eff27f</code></a> Prepare 9.1.1 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/80d96036277f0f8fe8dee27988db620afa925bfa"><code>80d9603</code></a> Refactored instant loading (<a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5032">#5032</a>)</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/7efb5fe70029933e232899642dfaf31dcbbe6de1"><code>7efb5fe</code></a> Updated Thai translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/48b89f3dc0796d5a2982c10635cd65fb5de4c3d2"><code>48b89f3</code></a> Updated Czech translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/091f9c07a8699feea7345fc66ca2150fcb27b234"><code>091f9c0</code></a> Updated Insiders changelog</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/4659d0a5eec9560438b1c4e0a19a0ef127108304"><code>4659d0a</code></a> Documentation</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/41f783faa452a818c2d33e7cf03ba712591c9bb3"><code>41f783f</code></a> Updated changelog</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/7b8b82e8569a3c23958027afbab71dffa308fc38"><code>7b8b82e</code></a> Prepare 9.1.0 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/15578c7d418a80d2cc0414dbba935a3154dda386"><code>15578c7</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/eb51f1c38712593970b730627c5c27164bcb87ac"><code>eb51f1c</code></a> Updated distribution files</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.0.0...9.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.0.0&new-version=9.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-03-07 00:01:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1281" class=".btn">#1281</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-git-revision-date-localized-plugin from 1.1.0 to 1.2.0 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-git-revision-date-localized-plugin](https://github.com/timvink/mkdocs-git-revision-date-localized-plugin) from 1.1.0 to 1.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/releases">mkdocs-git-revision-date-localized-plugin's releases</a>.</em></p>
<blockquote>
<h2>revision-date-localized v1.2.0</h2>
<h2>What's Changed</h2>
<p>Features:</p>
<ul>
<li>Add support for <code>mkdocs-gen-files</code> by <a href="https://github.com/timvink"><code>@​timvink</code></a> in <a href="https://github-redirect.dependabot.com/timvink/mkdocs-git-revision-date-localized-plugin/pull/102">timvink/mkdocs-git-revision-date-localized-plugin#102</a></li>
<li>Add new 'strict' option, closes <a href="https://github-redirect.dependabot.com/timvink/mkdocs-git-revision-date-localized-plugin/issues/108">#108</a> by <a href="https://github.com/timvink"><code>@​timvink</code></a> in <a href="https://github-redirect.dependabot.com/timvink/mkdocs-git-revision-date-localized-plugin/pull/110">timvink/mkdocs-git-revision-date-localized-plugin#110</a></li>
</ul>
<p>Documentation:</p>
<ul>
<li>
<ul>
<li>switch kebab typo to snake case by <a href="https://github.com/wd60622"><code>@​wd60622</code></a> in <a href="https://github-redirect.dependabot.com/timvink/mkdocs-git-revision-date-localized-plugin/pull/105">timvink/mkdocs-git-revision-date-localized-plugin#105</a></li>
</ul>
</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/wd60622"><code>@​wd60622</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/timvink/mkdocs-git-revision-date-localized-plugin/pull/105">timvink/mkdocs-git-revision-date-localized-plugin#105</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/compare/v1.1.0...v1.2.0">https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/compare/v1.1.0...v1.2.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/6150fad41a83abbf7500cf9c75696c5193532305"><code>6150fad</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/timvink/mkdocs-git-revision-date-localized-plugin/issues/110">#110</a> from timvink/108-strict-mode</li>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/7d89e01eb63a5d2a4ddaf220efc1460d41422b13"><code>7d89e01</code></a> Add pytz dependency for proper timezone support</li>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/e7f82dea3dd99742942064b85cf95a4c4e6902b3"><code>e7f82de</code></a> Add new 'strict' option, closes <a href="https://github-redirect.dependabot.com/timvink/mkdocs-git-revision-date-localized-plugin/issues/108">#108</a></li>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/7ddc74cb72c55a18d15cabead18a31ef243d490c"><code>7ddc74c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/timvink/mkdocs-git-revision-date-localized-plugin/issues/105">#105</a> from wd60622/kebab-case-typo</li>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/e915eedf45e199a168168d28480be284217331b6"><code>e915eed</code></a> switch kebab typo to snake case</li>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/6be250864f596242f4d24cc9544390252089fe25"><code>6be2508</code></a> ignore genfiles test for now</li>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/bbc9fdc0c011ae0d655a830dc17389b1ea47684d"><code>bbc9fdc</code></a> trigger ci</li>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/432220d685fbef1e7706c1888f75d43e06f9a161"><code>432220d</code></a> Merge branch 'master' of github.com:timvink/mkdocs-git-revision-date-localize...</li>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/1faaf2d61ea54ac4133ee9d46213bf746a537436"><code>1faaf2d</code></a> Add support for mkdocs-gen-files</li>
<li><a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/commit/ad11dd08a80422656e64fe56a6044fcec3b2742e"><code>ad11dd0</code></a> Create FUNDING.yml</li>
<li>Additional commits viewable in <a href="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/compare/v1.1.0...v1.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-git-revision-date-localized-plugin&package-manager=pip&previous-version=1.1.0&new-version=1.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-03-07 00:01:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1280" class=".btn">#1280</a>
            </td>
            <td>
                <b>
                    Update block parameter to include blockHash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document the `blockHash` option for block parameter, and minor updates to related content.

Fixes #1242

Preview: https://hyperledger-besu--1280.org.readthedocs.build/en/1280/public-networks/how-to/use-besu-api/json-rpc/#block-parameter
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 22:52:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1279" class=".btn">#1279</a>
            </td>
            <td>
                <b>
                    Add link to quorum plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add link to Quorum Plugins doc site from the `--security-module` CLI option.

See https://github.com/ConsenSys/doc.quorumplugins/issues/118
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 21:36:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1278" class=".btn">#1278</a>
            </td>
            <td>
                <b>
                    Update eth_feeHistory API.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Updates to the eth_feeHistory JSON-RPC API. 
- `blockCount` accepts an integer value as hex
- add missing array parameter
- add missing result key

## Issue fixed

Fixes #1269 

## Impacted parts

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

## Preview

https://hyperledger-besu--1278.org.readthedocs.build/en/1278/public-networks/reference/api/#eth_feehistory

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 01:45:25 +0000 UTC
    </div>
</div>

