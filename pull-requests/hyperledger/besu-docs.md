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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1277" class=".btn">#1277</a>
            </td>
            <td>
                <b>
                    Add RPC batch size CLI option
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

Add RPC batch size CLI option

## Issue fixed

Fixes #1258 

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

## Preview

https://hyperledger-besu--1277.org.readthedocs.build/en/1277/public-networks/reference/cli/options/#rpc-http-max-batch-size


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 01:17:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1276" class=".btn">#1276</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 9.0.0 to 9.0.15 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.0.0 to 9.0.15.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.1.0 (2023-02-??)</p>
<ul>
<li>Docker image now also built for arm64 and armv7</li>
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
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5061">#5061</a>: Improved discernibility of table row hover color</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5034">#5034</a>: Sequence actors in Mermaid diagrams not color-abiding</li>
<li>Fixed <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/4919">#4919</a>: Allow to hide version warning in multiple versions</li>
</ul>
<p>mkdocs-material-9.0.12+insiders-4.30.2 (2023-02-13)</p>
<ul>
<li>Fixed privacy plugin excludes not working (4.30.0 regression)</li>
</ul>
<p>mkdocs-material-9.0.12+insiders-4.30.1 (2023-02-12)</p>
<ul>
<li>Fixed privacy plugin not handling static templates e.g. 404.html</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/0f74615dc97e973eb83b4ade7d70ee68ad2550d7"><code>0f74615</code></a> Merge branch 'master' of github.com:squidfunk/mkdocs-material</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/a90f176e306c7617f0ce614c47f380060774e262"><code>a90f176</code></a> Prepare 9.0.15 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/175793163258367eb68a9fb4910785b6bc09778b"><code>1757931</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5088">#5088</a> from crazy-max/ci-refactor</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/8696f841bcd3fe6e30812982daa080f9131aa29a"><code>8696f84</code></a> Merge branch 'master' of github.com:squidfunk/mkdocs-material</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f3ae326e1a620e6ef84f37d41f5bf653f677f1a7"><code>f3ae326</code></a> Documentation</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/01377d23e34d0509c1e1de7b68362a396012f666"><code>01377d2</code></a> ci: bump docker/build-push-action to v4</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/cc0b4c5ec309658cff0143748d08fe050787ba2a"><code>cc0b4c5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/squidfunk/mkdocs-material/issues/5085">#5085</a> from mark-heptinstall/FixEditUriExample</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/a84029906521400d8438c0dd06e78aba91a6a574"><code>a840299</code></a> Updated Chinese (Traditional) translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/3e96638d462b71551c27ea05863f74576fc578b6"><code>3e96638</code></a> Merge branch 'master' of github.com:squidfunk/mkdocs-material</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/02f6699c34801c063d8d52515d412015d020047e"><code>02f6699</code></a> Updated Hebrew translations</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.0.0...9.0.15">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.0.0&new-version=9.0.15)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-02-28 00:02:25 +0000 UTC
    </div>
</div>

