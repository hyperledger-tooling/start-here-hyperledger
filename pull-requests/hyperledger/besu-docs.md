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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1256" class=".btn">#1256</a>
            </td>
            <td>
                <b>
                    Update config for tx-pool-limit-by-account-percentage on pub nets, consider moving to both sides 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the tx-pool-limit to the correct name for the parameter and provides a word of caution. Suggest that we copy this over to the private network side and call it out as well until we have a better parameterization default. We may be changing this shortly on Mainnet. I will ask @fab-10 to tag the docs team when he finishes his new transaction pool work. 

Signed-off-by: Matt Nelson <85905982+non-fungible-nelson@users.noreply.github.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 22:50:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1254" class=".btn">#1254</a>
            </td>
            <td>
                <b>
                    Bump plantuml-markdown from 3.8.0 to 3.8.1 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [plantuml-markdown](https://github.com/mikitex70/plantuml-markdown) from 3.8.0 to 3.8.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/releases">plantuml-markdown's releases</a>.</em></p>
<blockquote>
<h2>Added option for disabling SSL checks</h2>
<p>Added the 'insecure<code>configuration option to disable HTTPS SSL certificate validation. Set to</code>True` when using a custom PlantUML installation with self-signed certificates.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/blob/master/CHANGELOG.md">plantuml-markdown's changelog</a>.</em></p>
<blockquote>
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
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/79d5f7ba9ee9d7e98921ce1a1b09520da21de696"><code>79d5f7b</code></a> new: usr: added option for disabling SSL checks (refs <a href="https://github-redirect.dependabot.com/mikitex70/plantuml-markdown/issues/83">#83</a>)</li>
<li>See full diff in <a href="https://github.com/mikitex70/plantuml-markdown/compare/3.8.0...3.8.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=plantuml-markdown&package-manager=pip&previous-version=3.8.0&new-version=3.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-30 23:07:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1253" class=".btn">#1253</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 9.0.0 to 9.0.9 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.0.0 to 9.0.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
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
<h2>mkdocs-material-9.0.4</h2>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4823">#4823</a>: Improved contrast ratio in footer (9.0.2 regression)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4832">#4832</a>: Set navigation items back to black (9.0.3 regression)</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4843">#4843</a>: Emojis broken due to <code>maxcdn.com</code> shutting down</li>
<li>Upgraded Python Markdown Extensions to 9.9.1</li>
</ul>
<h2>mkdocs-material-9.0.3</h2>
<ul>
<li>Improved discernability of section index pages in navigation</li>
<li>Improved collapsing of adjacent whitespace in search plugin</li>
<li>Updated Indonesian translations</li>
<li>Fixed view source of this page button when edit URL points to blob</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4829">#4829</a>: Search overlay does not close for active anchor result</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4824">#4824</a>: Search plugin crashes for <code>h[1-6]</code> contained in other elements</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4804">#4804</a>: Nested navigation items not expandable with keyboard</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4689">#4689</a>: anchor tracking not working for anchors in tables</li>
<li>Upgraded to Mermaid 9.3.0</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
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
<li>Updated Polish and Portuguese (Brasilian) translations</li>
<li>Fixed info plugin terminating on subsequent reload when serving</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4910">#4910</a>: Sidebar navigation labels have invalid ARIA roles</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4884">#4884</a>: Search query terms can't be separated by colons</li>
</ul>
<p>mkdocs-material-9.0.6+insiders-4.29.0 (2023-01-21)</p>
<ul>
<li>Added built-in optimize plugin for automatically compressing images</li>
<li>Switched reporting in built-in privacy plugin to info level</li>
</ul>
<p>mkdocs-material-9.0.6 (2023-01-19)</p>
<ul>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4883">#4883</a>: Automatically disable info plugin when serving</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4885">#4885</a>: Search plugin crashes in some exotic cases (9.0.3 regression)</li>
</ul>
<p>mkdocs-material-9.0.5+insiders-4.28.1 (2023-01-17)</p>
<ul>
<li>Fixed built-in info plugin erroring for Insiders on version check</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4865">#4865</a>: Navigation paths render bug when there's no top-level section</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4875">#4875</a>: Added support for hiding navigation paths</li>
<li>Improved navigation path to not render for a single item</li>
</ul>
<p>mkdocs-material-9.0.5+insiders-4.28.0 (2023-01-14)</p>
<ul>
<li>Added support for navigation path (breadcrumbs)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/00175e38986d915c8ebf438a9c010dd37be3326e"><code>00175e3</code></a> Prepare 9.0.9 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/109614b6126e2f6c6be3f8fde0a652c9d5d508a0"><code>109614b</code></a> Fixed computation of missing translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/97b4798dd66d078f450809dc79b04a1bef217cf8"><code>97b4798</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/be0e198a49593aeef7486cf33b2c65d2d692079d"><code>be0e198</code></a> Updated Chinese (Simplified) translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/2747293403e013afd54330c268f7ec7d916b02df"><code>2747293</code></a> Updated Polish translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/567419b17fd5915ad538492fcf30ca4eb1d4de6b"><code>567419b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4958">#4958</a> from evetion/patch-1</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/3104df5fb26f83ea7e88b0abae4f359e0779e622"><code>3104df5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4957">#4957</a> from kamilkrzyskow/update-pl-lang2</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/d1d918d0764fb8327aac7beea5eb496bb28f3bc4"><code>d1d918d</code></a> Fix Dutch translation of contributors.</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/3db06ad8b4b0bffc871669abd8fbb6aaf1168130"><code>3db06ad</code></a> Updated translation template</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/557eaac71c21ef1624a630b02fb1d70d881859f5"><code>557eaac</code></a> Merge branch 'master' of github.com:squidfunk/mkdocs-material</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.0.0...9.0.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.0.0&new-version=9.0.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-30 23:07:00 +0000 UTC
    </div>
</div>

