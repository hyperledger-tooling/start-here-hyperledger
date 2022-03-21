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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/991" class=".btn">#991</a>
            </td>
            <td>
                <b>
                    Bump mkdocs from 1.1.2 to 1.2.3 in /CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mkdocs](https://github.com/mkdocs/mkdocs) from 1.1.2 to 1.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mkdocs/mkdocs/releases">mkdocs's releases</a>.</em></p>
<blockquote>
<h2>1.2.3</h2>
<p>MkDocs 1.2.3 is a bugfix release for <a href="https://www.mkdocs.org/about/release-notes/#version-12-2021-06-04">MkDocs 1.2</a>.</p>
<p><em>Aside</em>: MkDocs has a new <a href="https://gitter.im/mkdocs/community">chat room</a> on Gitter/Matrix. <a href="https://github.com/mkdocs/mkdocs#support">More details</a>.</p>
<p>Improvements:</p>
<ul>
<li>
<p>Built-in themes now also support these languages:</p>
<ul>
<li>Simplified Chinese (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2497">#2497</a>)</li>
<li>Japanese (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2525">#2525</a>)</li>
<li>Brazilian Portuguese (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2535">#2535</a>)</li>
<li>Spanish (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2545">#2545</a>, previously <a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2396">#2396</a>)</li>
</ul>
</li>
<li>
<p>Third-party plugins will take precedence over built-in plugins with the same name (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2591">#2591</a>)</p>
</li>
<li>
<p>Bugfix: Fix ability to load translations for some languages: core support (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2565">#2565</a>) and search plugin support with fallbacks (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2602">#2602</a>)</p>
</li>
<li>
<p>Bugfix (regression in 1.2): Prevent directory traversal in the dev server (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2604">#2604</a>)</p>
</li>
<li>
<p>Bugfix (regression in 1.2): Prevent webserver warnings from being treated as a build failure in strict mode (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2607">#2607</a>)</p>
</li>
<li>
<p>Bugfix: Correctly print colorful messages in the terminal on Windows (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2606">#2606</a>)</p>
</li>
<li>
<p>Bugfix: Python version 3.10 was displayed incorrectly in <code>--version</code> (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2618">#2618</a>)</p>
</li>
</ul>
<p>Other small improvements; see <a href="https://github.com/mkdocs/mkdocs/compare/1.2.2...1.2.3">commit log</a>.</p>
<h2>1.2.2</h2>
<p>MkDocs 1.2.2 is a bugfix release for <a href="https://www.mkdocs.org/about/release-notes/#version-12-2021-06-04">MkDocs 1.2</a> -- make sure you've seen the &quot;major&quot; release notes as well.</p>
<ul>
<li>
<p>Bugfix (regression in 1.2): Fix serving files/paths with Unicode characters (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2464">#2464</a>)</p>
</li>
<li>
<p>Bugfix (regression in 1.2): Revert livereload file watching to use polling observer (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2477">#2477</a>)</p>
<p>This had to be done to reasonably support usages that span virtual filesystems such as non-native Docker and network mounts.</p>
<p>This goes back to the polling approach, very similar to that was always used prior, meaning most of the same downsides with latency and CPU usage.</p>
</li>
<li>
<p>Revert from 1.2: Remove the requirement of a <code>site_url</code> config and the restriction on <code>use_directory_urls</code> (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2490">#2490</a>)</p>
</li>
<li>
<p>Bugfix (regression in 1.2): Don't require trailing slash in the URL when serving a directory index in <code>mkdocs serve</code> server (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2507">#2507</a>)</p>
<p>Instead of showing a 404 error, detect if it's a directory and redirect to a path with a trailing slash added, like before.</p>
</li>
<li>
<p>Bugfix: Fix <code>gh_deploy</code> with config-file in the current directory (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2481">#2481</a>)</p>
</li>
<li>
<p>Bugfix: Fix reversed breadcrumbs in &quot;readthedocs&quot; theme (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2179">#2179</a>)</p>
</li>
<li>
<p>Allow &quot;mkdocs.yaml&quot; as the file name when '--config' is not passed (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2478">#2478</a>)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mkdocs/mkdocs/commit/d167eab473c1b772f0d5f999d580c8bf3ef9b59f"><code>d167eab</code></a> Release 1.2.3 (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2614">#2614</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs/commit/5629b09f1a04fdfbbf0704b502c231ec255257ad"><code>5629b09</code></a> Re-format translation files to pass a lint check (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2621">#2621</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs/commit/2c4679b00a4484caa13eef06318652c09e147524"><code>2c4679b</code></a> Re-format translation files to pass a lint check (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2620">#2620</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs/commit/9262cc576dede2203edb57db26e8c17115f42035"><code>9262cc5</code></a> Fix the code to abbreviate Python's version (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2618">#2618</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs/commit/83458500608d41af04c07c6cbb20eb6b5072f571"><code>8345850</code></a> Add hint about <code>-f/--config-file</code> in configuration documentation (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2616">#2616</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs/commit/815af480d64cc8232bfbd3f722db63752956a149"><code>815af48</code></a> Added translation for Brazilian Portuguese (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2535">#2535</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs/commit/6563439956409ca691b5df0fb8fccfc91b5a4056"><code>6563439</code></a> Update contact instructions: announce chat, preference for issues (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2610">#2610</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs/commit/6b72eef74852d105988e83e0c50fa3c901cc53c1"><code>6b72eef</code></a> We can again announce support of zh_CN locale (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2609">#2609</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs/commit/b18ae296593cbc35c6c329a294c3c3c21687ec58"><code>b18ae29</code></a> Drop <code>assert_mock_called_once</code> compat method from tests (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2611">#2611</a>)</li>
<li><a href="https://github.com/mkdocs/mkdocs/commit/7a27572d0e41f0e78239f93693b12b9236eb9905"><code>7a27572</code></a> Isolate strict warning counter to just the ongoing build (<a href="https://github-redirect.dependabot.com/mkdocs/mkdocs/issues/2607">#2607</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/mkdocs/mkdocs/compare/1.1.2...1.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs&package-manager=pip&previous-version=1.1.2&new-version=1.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/besu-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 19:24:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/990" class=".btn">#990</a>
            </td>
            <td>
                <b>
                    Bump node-fetch from 2.6.1 to 2.6.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 2.6.1 to 2.6.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/releases">node-fetch's releases</a>.</em></p>
<blockquote>
<h2>v2.6.7</h2>
<h1>Security patch release</h1>
<p>Recommended to upgrade, to not leak sensitive cookie and authentication header information to 3th party host while a redirect occurred</p>
<h2>What's Changed</h2>
<ul>
<li>fix: don't forward secure headers to 3th party by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1453">node-fetch/node-fetch#1453</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7">https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7</a></p>
<h2>v2.6.6</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(URL): prefer built in URL version when available and fallback to whatwg by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1352">node-fetch/node-fetch#1352</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6">https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6</a></p>
<h2>v2.6.2</h2>
<p>fixed main path in package.json</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/1ef4b560a17e644a02a3bfdea7631ffeee578b35"><code>1ef4b56</code></a> backport of <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1449">#1449</a> (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1453">#1453</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8fe5c4ea66b9b8187600e6d5ec9b1b6781f44009"><code>8fe5c4e</code></a> 2.x: Specify encoding as an optional peer dependency in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1310">#1310</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/f56b0c66d3dd2ef185436de1f2fd40f66bfea8f4"><code>f56b0c6</code></a> fix(URL): prefer built in URL version when available and fallback to whatwg (...</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/b5417aea6a3275932283a200214522e6ab53f1ea"><code>b5417ae</code></a> fix: import whatwg-url in a way compatible with ESM Node (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1303">#1303</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/18193c5922c64046b922e18faf41821290535f06"><code>18193c5</code></a> fix v2.6.3 that did not sending query params (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1301">#1301</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/ace7536c955556be742d9910566738630cc3c2a6"><code>ace7536</code></a> fix: properly encode url with unicode characters (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1291">#1291</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/152214ca2f6e2a5a17d71e4638114625d3be30c6"><code>152214c</code></a> Fix(package.json): Corrected main file path in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1274">#1274</a>)</li>
<li>See full diff in <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.1...v2.6.7">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~endless">endless</a>, a new releaser for node-fetch since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=2.6.1&new-version=2.6.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/besu-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 19:23:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/989" class=".btn">#989</a>
            </td>
            <td>
                <b>
                    initial merge documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexandra Tran <alexandra.tran@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [x] you fixed all the issues raised by the tests, if any.
- [x] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change

<!-- A clear and concise description of what this PR changes in the documentation. -->

Doc conceptual merge information and how to join Kiln testnet. Minor merge-related updates throughout docs.

## Issue fixed

<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

fixes #985 
fixes #981 
fixes #984

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing

<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->

https://hyperledger-besu--989.org.readthedocs.build/en/989/Concepts/Merge/

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 06:49:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/988" class=".btn">#988</a>
            </td>
            <td>
                <b>
                    Remove caution about not being able to change the miningbeneficiary in a running network for BFT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following https://github.com/hyperledger/besu-docs/pull/973

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [x] you fixed all the issues raised by the tests, if any.
- [x] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

## Testing

<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->
https://hyperledger-besu--988.org.readthedocs.build/en/988/HowTo/Configure/Consensus-Protocols/QBFT/#genesis-file
https://hyperledger-besu--988.org.readthedocs.build/en/988/HowTo/Configure/Consensus-Protocols/IBFT/#genesis-file
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 00:23:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/987" class=".btn">#987</a>
            </td>
            <td>
                <b>
                    Update milestone information in genesis file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roland Tyler <roland.tyler@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [x] you fixed all the issues raised by the tests, if any.
- [x] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change
Update milestone examples
Add recommendation to use latest milestone for private networks.
<!-- A clear and concise description of what this PR changes in the documentation. -->

## Issue fixed
Fixes #972 
<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing

<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 20:44:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/986" class=".btn">#986</a>
            </td>
            <td>
                <b>
                    Update Trace APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roland Tyler <roland.tyler@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [x] you fixed all the issues raised by the tests, if any.
- [x] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change
PR 971 was merged before corrections. This PR addresses that feedback.

- Update pruned blocks language for clarity
- Fix code error in `trace-get`
- fix code error in `trace-rawTransaction`

<!-- A clear and concise description of what this PR changes in the documentation. -->

## Issue fixed
See #971 
<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing
https://hyperledger-besu--986.org.readthedocs.build/en/971/HowTo/Troubleshoot/Trace-Transactions/
https://hyperledger-besu--986.org.readthedocs.build/en/971/Reference/API-Methods/#trace-methods
<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 17:36:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/983" class=".btn">#983</a>
            </td>
            <td>
                <b>
                    doc bonsai options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexandra Tran <alexandra.tran@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [ ] you fixed all the issues raised by the tests, if any.
- [ ] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change

<!-- A clear and concise description of what this PR changes in the documentation. -->

Doc unhidden Bonsai CLI options. Remove "Configure data storage" page in favor of CLI documentation. Minor format edits throughout CLI page.

## Issue fixed

<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

fixes #979 

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing

<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->

## Screenshots / recording

<!-- If it helps understanding your change,
don't hesitate to link an annotated screenshot or a small demo video. -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 04:39:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/978" class=".btn">#978</a>
            </td>
            <td>
                <b>
                    [MINOR] delete spurious comma
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Removed extra comma in genesis file example

- [x] Doc content
- [ ] Doc pages organisation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 23:26:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/977" class=".btn">#977</a>
            </td>
            <td>
                <b>
                    Update enterprise description
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roland Tyler <roland.tyler@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [x] you fixed all the issues raised by the tests, if any.
- [x] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change
Update index page to shift focus from enterprise Ethereum to public networks
<!-- A clear and concise description of what this PR changes in the documentation. -->

## Issue fixed
Fixes #976 
<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing

<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->

## Screenshots / recording

<!-- If it helps understanding your change,
don't hesitate to link an annotated screenshot or a small demo video. -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 18:24:20 +0000 UTC
    </div>
</div>

