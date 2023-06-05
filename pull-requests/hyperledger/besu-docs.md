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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1339" class=".btn">#1339</a>
            </td>
            <td>
                <b>
                    Txpool options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #568 # Pull request checklist

Document missing transaction pool CLI options.

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

## After creating your PR and tests have finished

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

https://hyperledger-besu--1339.org.readthedocs.build/en/1339/public-networks/reference/cli/options/#tx-pool-disable-locals
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 03:06:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1338" class=".btn">#1338</a>
            </td>
            <td>
                <b>
                    mkdocs to docusaurus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

Major changes to switch mkdocs -> docusaurus

### Before creating the pull request

Make sure that:

- [X] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [X] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

- Removing mkdocs and switching to docusaurus
- Removing old versions from the versions list (still available as code though)
- updating to use GHA 
- will need to be set to use github pages
## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [X] Documentation content
- [X] Documentation page organization

For tool changes:

- [x] Github Actions workflow
- [x] Build and QA tools configuration (for example, lint rules or Vale style)
- [x] MkDocs templates
- [x] MkDocs configuration
- [x] Python dependencies
- [x] Node dependencies and JavaScript
- [x] Read the Docs configuration
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
        Created At 2023-05-31 01:13:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1337" class=".btn">#1337</a>
            </td>
            <td>
                <b>
                    Add link to staking calculator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Adding a link to Staking Rewards calculator for validators to see what they can expect to be rewarded.
## Issue fixed

None

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
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 21:13:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1336" class=".btn">#1336</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 9.1.14 to 9.1.15 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.1.14 to 9.1.15.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.1.15</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5566">#5566</a>: Indicate color scheme to operating system</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5565">#5565</a>: Update <code>Dockerfile</code> to latest version of base image</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5554">#5554</a>: Add additional version tags (<code>9</code>, <code>9.1</code>) to Docker image</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5536">#5536</a>: Strip tags of ARIA labels in table of contents</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.1.15+insiders-4.35.2 (2023-05-29)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5555">#5555</a>: Blog plugin crashes when computing readtime for emojis</li>
</ul>
<p>mkdocs-material-9.1.15 (2023-05-29)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5566">#5566</a>: Indicate color scheme to operating system</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5565">#5565</a>: Update Dockerfile to latest version of base image</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5554">#5554</a>: Add additional version tags (9, 9.1) to Docker image</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5536">#5536</a>: Strip tags of ARIA labels in table of contents</li>
</ul>
<p>mkdocs-material-9.1.14+insiders-4.35.1 (2023-05-20)</p>
<ul>
<li>Fixed internal handling of errors in social plugin</li>
</ul>
<p>mkdocs-material-9.1.14+insiders-4.35.0 (2023-05-20)</p>
<ul>
<li>Improve editing experience and stability of social plugin</li>
<li>Added support for custom layout syntax validation in social plugin</li>
<li>Added support for layer origin for easier placement in social plugin</li>
<li>Added support for in- and exclusion patterns in social plugin</li>
<li>Catch and print syntax errors in custom layouts</li>
</ul>
<p>mkdocs-material-9.1.14 (2023-05-20)</p>
<ul>
<li>Updated Armenian and Greek translations</li>
</ul>
<p>mkdocs-material-9.1.13+insiders-4.34.1 (2023-05-16)</p>
<ul>
<li>Disable social plugin debug mode by default on mkdocs build</li>
<li>Added warning in social plugin debug mode when font style couldn't be found</li>
<li>Set default concurrency of built-in multi-threaded plugins to CPUs - 1</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5521">#5521</a>: Social plugin triggers race condition when downloading fonts</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5515">#5515</a>: Social plugin crashes when concurrency is set to 1</li>
</ul>
<p>mkdocs-material-9.1.13 (2023-05-16)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5517">#5517</a>: Social plugin crashes for some fonts (e.g. Open Sans)</li>
</ul>
<p>mkdocs-material-9.1.12+insiders-4.34.0 (2023-05-14)</p>
<ul>
<li>Added support for new overflow mode to auto-fit text in social plugin</li>
<li>Reduced subtle rendering bugs in (code) annotations due to subpixel rounding</li>
<li>Improved print styles for (code) annotation lists</li>
<li>Improved performance of social plugin, now 3x as fast</li>
<li>Improved interop of typeset plugin with MkDocstrings</li>
<li>Fixed logo location for variants of default template in social plugin</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5446">#5446</a>: Built-in typeset plugin picks up headings in code blocks</li>
</ul>
<p>mkdocs-material-9.1.12+insiders-4.33.2 (2023-05-12)</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/06d1ba1337703bd6deed9b13b33516abc2e81b72"><code>06d1ba1</code></a> Prepare 9.1.15 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/3d706407d96fbc7d87b11f24da13d389e6879c36"><code>3d70640</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/0f1866b108d06eb18f9610f211439badb41cbca1"><code>0f1866b</code></a> Documentation</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/aa4befa429971e9e55af09c5021f9f9b2340a05d"><code>aa4befa</code></a> Merge branch 'master' of github.com:squidfunk/mkdocs-material</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/fe0c966a4da16861e3fbe9064afcae3cc3d7c6fa"><code>fe0c966</code></a> Added color-scheme property to indicate color scheme to OS</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/2fa92de28dd4f455f6206c958e79cbec1203bc98"><code>2fa92de</code></a> Merge pull request <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5565">#5565</a> from yubiuser/update_docker</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/7c19f464ad5b42bb2497785b3a12ecc0daa95206"><code>7c19f46</code></a> Only user major.minor for python version</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f37702a8fbb62ee35e45f57a462d8be540856c44"><code>f37702a</code></a> Added major.minor and major tags to Docker image</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/e0b3022be64456442aa51a90c57a8530998d576e"><code>e0b3022</code></a> Update Dockerfile to latest alpine</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f84725d4fcd8960090063d58f18fb01973b55370"><code>f84725d</code></a> Added tutorial on building custom social cards</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.1.14...9.1.15">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.1.14&new-version=9.1.15)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-05-29 23:58:38 +0000 UTC
    </div>
</div>

