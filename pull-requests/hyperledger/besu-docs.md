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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1316" class=".btn">#1316</a>
            </td>
            <td>
                <b>
                    Updates for peering page.
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

- [X] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [X] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [X] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change
 Minor edits for peering page 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 18:12:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1315" class=".btn">#1315</a>
            </td>
            <td>
                <b>
                    Bump plantuml-markdown from 3.8.3 to 3.9.0 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [plantuml-markdown](https://github.com/mikitex70/plantuml-markdown) from 3.8.3 to 3.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/releases">plantuml-markdown's releases</a>.</em></p>
<blockquote>
<h2>Added two new configuration options</h2>
<p>Added the following configuration options:</p>
<ul>
<li><code>config</code>: set the PlantUML configuration file (as the <code>-config</code> plantuml command line option)</li>
<li><code>plantuml_cmd</code>: set the plantuml command to execute (defaults to <code>plantuml</code>); can be used for passing custom options to java, for example <code>java -Dplantuml.include.path=includes -jar plantuml.jar</code>.</li>
</ul>
<p>See the <code>README.md</code> for more details.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mikitex70/plantuml-markdown/blob/master/CHANGELOG.md">plantuml-markdown's changelog</a>.</em></p>
<blockquote>
<h2>3.9.0 (2023-04-23)</h2>
<h3>New</h3>
<ul>
<li>
<p>Added support for other plantuml diagrams. [Michele Tessaro]</p>
<p>Now can be used other kind of diagrams, like <code>startgantt</code>,
<code>startmindmap</code>, <code>startjson</code> and many others.</p>
</li>
<li>
<p>Added option for overriding plantuml command (resolves <a href="https://redirect.github.com/mikitex70/plantuml-markdown/issues/87">#87</a>) [Michele Tessaro]</p>
</li>
<li>
<p>Added plantuml config option (implements <a href="https://redirect.github.com/mikitex70/plantuml-markdown/issues/88">#88</a>) [Michele Tessaro]</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/6d8efd09c6f14298f9b47a4f51776a6aa3d3fc38"><code>6d8efd0</code></a> chg: pkg: changed version for the new release</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/6cc35458b637c8d167acdb44b5a3e26fae8f4fa4"><code>6cc3545</code></a> fix: test: fixed tests with latest plantuml release</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/227e934bbb1aa8ae3f9f5ba977831c40e283a38c"><code>227e934</code></a> new: usr: added support for other plantuml diagrams</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/ec5e13d3033a5f3c9ea51706d29dcffe4aa73891"><code>ec5e13d</code></a> new: usr: added option for overriding plantuml command (resolves <a href="https://redirect.github.com/mikitex70/plantuml-markdown/issues/87">#87</a>)</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/3f8f6c758b20902ed4ee676838fe152f585aaebc"><code>3f8f6c7</code></a> fix: dev: fixed declaration of static method</li>
<li><a href="https://github.com/mikitex70/plantuml-markdown/commit/b4bed608a4d24c68c507ba8ea9e800b20beb7b6e"><code>b4bed60</code></a> new: usr: added plantuml config option (implements <a href="https://redirect.github.com/mikitex70/plantuml-markdown/issues/88">#88</a>)</li>
<li>See full diff in <a href="https://github.com/mikitex70/plantuml-markdown/compare/3.8.3...3.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=plantuml-markdown&package-manager=pip&previous-version=3.8.3&new-version=3.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-04-24 23:58:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1314" class=".btn">#1314</a>
            </td>
            <td>
                <b>
                    Bump mkdocs-material from 9.1.6 to 9.1.8 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.1.6 to 9.1.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.1.8</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5417">#5417</a>: Theme breaks when <code>palette</code> is not defined (9.1.7 regression)</li>
</ul>
<h2>mkdocs-material-9.1.7</h2>
<ul>
<li>Updated Persian (Farsi) and Turkish translations</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5401">#5401</a>: Added missing flag to disable built-in tags plugin</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5206">#5206</a>: Ensure defaults are set for primary and accent colors</li>
<li>Fixed unnecessary inclusion of palette CSS when unused</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
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
<li>Updated Mermaid.js to version 9.4.3</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5290">#5290</a>: Footer previous/next labels cut-off for short page titles</li>
</ul>
<p>mkdocs-material-9.1.4+insiders-4.32.4 (2023-03-24)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5241">#5241</a>: Built-in typeset plugin jams navigation for anchors in headings</li>
</ul>
<p>mkdocs-material-9.1.4 (2023-03-24)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5239">#5239</a>: Instant loading breaks anchors in details (9.1.1 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5211">#5211</a>: Anchor following not working for Chinese (9.1.2 regression)</li>
</ul>
<p>mkdocs-material-9.1.3 (2023-03-14)</p>
<ul>
<li>Added Kurdish (Soranî) translations</li>
<li>Updated Norwegian (Bokmål), Portuguese and Romanian translations</li>
<li>Improved compatibility with mkdocs-jupyter plugin</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5198">#5198</a>: Built-in search plugin not filtering script and style tags</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5176">#5176</a>: Back-to-top + instant loading not working (9.1.1 regression)</li>
</ul>
<p>mkdocs-material-9.1.2+insiders-4.32.3 (2023-03-09)</p>
<ul>
<li>Fixed Docker image release workflow (9.1.0 regression)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/2ac2cbc3ae2358767d1311797f9a185540f83271"><code>2ac2cbc</code></a> Prepare 9.1.8 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f0d506c4461d5f3ed41b65ffe051dd2b018dac0d"><code>f0d506c</code></a> Fixed theme breaking when no palette is defined</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/0028518f1a062a66d0b42ad5b74093cca936b3b7"><code>0028518</code></a> Prepare 9.1.7 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/6398f529d60e4c0e3b1b97a2b62ba1fd56c4bcc3"><code>6398f52</code></a> Merge branch 'master' of github.com:squidfunk/mkdocs-material</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/6f13021a3824a63c7b7b9f0136c945753f10d738"><code>6f13021</code></a> Fixed unnecessary inclusion of palette.css</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/6fe1d556071416122af362064c78873babcfe9cf"><code>6fe1d55</code></a> Always set default primary and accent colors</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/207fd4029f3870c73b9a86c78bb89aaca8b83cf9"><code>207fd40</code></a> Merge pull request <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5389">#5389</a> from robingenz/patch-1</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/ba90cb1ccda74118bcf694c28e32fb1570ec8ea1"><code>ba90cb1</code></a> Added missing enabled setting for tags plugin</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/c0cdb3ca1f7ce1cf85d021f39733c8ea14244c9a"><code>c0cdb3c</code></a> Updated Turkish translations</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/ab94f5f648d8b781461c77a901458e142d8d4277"><code>ab94f5f</code></a> Updated Persian (Farsi) translations</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.1.6...9.1.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.1.6&new-version=9.1.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-04-24 23:58:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1312" class=".btn">#1312</a>
            </td>
            <td>
                <b>
                    Adding new peering trobuleshooting page.
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
- [ ] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Adding peering FAQ

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
        Created At 2023-04-20 16:27:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1311" class=".btn">#1311</a>
            </td>
            <td>
                <b>
                    Update attestation page and add some references
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
- [ ] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Update the attestation page and add some references

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
        Created At 2023-04-20 14:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1310" class=".btn">#1310</a>
            </td>
            <td>
                <b>
                    Adding new attestations page, credit Amez/Ben.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Before creating the pull request

Make sure that:

- [X] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [X] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [X] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Adding page for attestations and changing proof of stake structure. 

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
        Created At 2023-04-19 18:13:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1308" class=".btn">#1308</a>
            </td>
            <td>
                <b>
                    Update Grafana link to point to Besu Full dashboard
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
- [ ] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

Update Grafana link to point to Besu Full dashboard instead of Besu Overview since that is more useful for users to debug Besu with.

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
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

https://hyperledger-besu--1308.org.readthedocs.build/en/1308/public-networks/how-to/monitor/metrics/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 00:22:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1306" class=".btn">#1306</a>
            </td>
            <td>
                <b>
                    remove launcher doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove reference to launcher CLI
See https://github.com/hyperledger/besu/pull/5355

- [x] Documentation content
- [ ] Documentation page organization

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

https://hyperledger-besu--1306.org.readthedocs.build/en/1306/public-networks/get-started/start-node/

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 19:38:01 +0000 UTC
    </div>
</div>

